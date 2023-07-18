# Comparing `tmp/dopplrSDK-3.2.0-py3-none-any.whl.zip` & `tmp/dopplrSDK-3.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5490 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    12871 b- defN 23-Jul-17 11:28 dopplrSDK/__init__.py
--rw-rw-rw-  2.0 fat     1077 b- defN 23-Jul-17 11:38 dopplrSDK-3.2.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      622 b- defN 23-Jul-17 11:38 dopplrSDK-3.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-17 11:38 dopplrSDK-3.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-17 11:38 dopplrSDK-3.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      478 b- defN 23-Jul-17 11:38 dopplrSDK-3.2.0.dist-info/RECORD
-6 files, 15150 bytes uncompressed, 4624 bytes compressed:  69.5%
+Zip file size: 6183 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    13023 b- defN 23-Jul-18 09:53 dopplrSDK/__init__.py
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-Jul-18 09:54 dopplrSDK-3.3.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     2246 b- defN 23-Jul-18 09:54 dopplrSDK-3.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-18 09:54 dopplrSDK-3.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-18 09:54 dopplrSDK-3.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      479 b- defN 23-Jul-18 09:54 dopplrSDK-3.3.0.dist-info/RECORD
+6 files, 16927 bytes uncompressed, 5317 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: dopplrSDK/__init__.py
 Comment: 
 
-Filename: dopplrSDK-3.2.0.dist-info/LICENSE.txt
+Filename: dopplrSDK-3.3.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dopplrSDK-3.2.0.dist-info/METADATA
+Filename: dopplrSDK-3.3.0.dist-info/METADATA
 Comment: 
 
-Filename: dopplrSDK-3.2.0.dist-info/WHEEL
+Filename: dopplrSDK-3.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: dopplrSDK-3.2.0.dist-info/top_level.txt
+Filename: dopplrSDK-3.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dopplrSDK-3.2.0.dist-info/RECORD
+Filename: dopplrSDK-3.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dopplrSDK/__init__.py

```diff
@@ -21,19 +21,23 @@
     cipher = DES3.new(key1, DES3.MODE_ECB)
     decrypted_bytes = cipher.decrypt(cipher_bytes)
     decrypted_text = unpad(decrypted_bytes, DES3.block_size).decode("utf-8")
     data=decrypted_text.split('|')
     
     for i in data:
         a=i.split(':')
-        keys[a[0]]=a[1]
+        if len(a)==3:
+            keys[a[0]]=a[1]+':'+a[2]          
+        else:
+            keys[a[0]]=a[1]
+
     Cloud=keys['Cloud']
     if Cloud == 'MinIO':
         endpoint_url=keys['endpoint_url']
-        s3=boto3.client('s3',endpoint_url=f"http://{endpoint_url}:9000",
+        s3=boto3.client('s3',endpoint_url=f"http://{endpoint_url}",
                       aws_access_key_id=keys['Access'],
                       aws_secret_access_key=keys['Secret'],
                       config=Config(signature_version='s3v4'),region_name=keys['region_name']
                       )   
         
     elif Cloud == 'AWS':
         s3 = boto3.client('s3', aws_access_key_id=keys['Access'], aws_secret_access_key=keys['Secret'])
@@ -83,41 +87,36 @@
 
 def putFileTomywrkspace(filePath,file_type,loginName,Project_name,de_key):
     try:
         keys,db,client=decrypt_keys(de_key)
         api=db['api']
         fapi=db['fastapi']
         Cloud=keys['Cloud']
-        
-
-
         query="select DOR.\"OrgName\",Du.\"UserKey\",P.\"Project_key\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" \
 join doppler.\"DopplerProject\" P on P.\"UserKey\"=Du.\"UserKey\" where Du.\"LoginName\"='{0}' and p.\"ProjectName\"='{1}'".format(loginName,Project_name)
         
         ContainerName = keys['Bucket']
         cnxn = psycopg2.connect(host=db['host'],database=db['database'],user=db['user'],password=db['password'],port=db['port'])
     
         cur=cnxn.cursor()
         cur.execute(query)
         results = cur.fetchone()
-        
-        
+
         OrgName=results[0]
+        
         UserKey=results[1]
         ProjectKey=results[2]
         
         cur=cnxn.cursor()
         file_name = os.path.basename(filePath)
-
         query="select count(\"TableName\") from doppler.\"DopplerLake\" DL join doppler.\"DopplerUser\" US on DL.\"UserKey\"=US.\"UserKey\" where \"TableName\"="+"'"+file_name+"'"+" and US.\"LoginName\"="+"'"+loginName+"'"
-        print(query)
         cur.execute(query)
         results = cur.fetchone()
         if results[0]<1:
-
+        
             insert_query = "INSERT INTO doppler.\"DopplerLake\"(\"UserKey\", \"TableName\",\"ResourceType\",\"DopplerConnectionDetailsKey\",\"Projectid\",\"Status\") VALUES ("+str(UserKey)+",'"+file_name+"','"+file_type+"',null,'"+str(ProjectKey)+"','Uploaded')"
             cur.execute(insert_query)
             cnxn.commit()
         else:
             pass
                     
         cur1=cnxn.cursor()
@@ -141,15 +140,15 @@
             tpp=str(maxlength)
             tp=str(dtype)
             insert1="INSERT INTO doppler.\"DopplerSchema\"(\"SourceKey\",\"Column\" ,\"Type\",\"Length\") VALUES ({},'{}','{}','{}')".format(SourceKey,name,tp,tpp)
             cur_sch.execute(insert1)
             cnxn.commit()
 
         ConnectionString = str(OrgName)+"/"+str(loginName).upper()+"/"+(str(SourceKey).lstrip()+'/Source/'+file_name+'.'+file_type)
-        update_query = "UPDATE doppler.\"DopplerLake\" set \"ConnectionString\"='"+str(OrgName)+"/"+str(loginName).upper()+'/'+(str(SourceKey).lstrip()+'/Source/'+file_name+'.'+file_type+"',\"Source\"= 'MLStudio' ,\"Status\"='Uploaded',\"CreatedTs\"=CURRENT_TIMESTAMP where \"SourceKey\"="+str(SourceKey))
+        update_query = "UPDATE doppler.\"DopplerLake\" set \"ConnectionString\"='"+ConnectionString+"',"+"\"Schema\"='"+loginName+'_schema'+"',\"Source\"= 'MLStudio' ,\"Status\"='Uploaded',\"CreatedTs\"=CURRENT_TIMESTAMP where \"SourceKey\"="+str(SourceKey)
         cur2=cnxn.cursor()
 
         cur2.execute(update_query)
         cnxn.commit()
         #print("uploaded")
 
         
@@ -170,28 +169,31 @@
                 'get_object',
                 Params={
                     'Bucket': ContainerName,
                     'Key': ConnectionString
                 },
                 ExpiresIn=3600  # URL expiration time in seconds (e.g., 1 hour)
             )
-            url = f"http://{endpoint_url}:9000/{ContainerName}/{ConnectionString}"            
+            url = presigned_url#f"http://{endpoint_url}/{ContainerName}/{ConnectionString}"            
             print("uri : ",url)
         else:
             #print(keys['Cloud'])
             blob_client = client.get_blob_client(container=ContainerName, blob=file_name)
             with open(filePath+'.'+file_type, "rb") as data:
                 blob_client.upload_blob(data)
             
         cnxn.close()
         api=f"http://{api}/Workflow/WorkflowDruidSave?SourceID="+(str(SourceKey).lstrip())
+        #print("api : ",api)
         response=requests.get(api,verify=False)
+        #print("response ",response)
         fapi=f"http://{fapi}/Profiling/?sourcekey="+(str(SourceKey).lstrip())
+        #print("Profiling call : ",fapi)
         response=requests.get(fapi,verify=False)
-       
+        #print("response1 ",response)
 
         
             
     except Exception as error:
         if 'NoneType' in str(error):
             dopplrsource= 'File does not exists'
             print("Error : ", dopplrsource)
@@ -288,7 +290,8 @@
                     file.write(blob_client.download_blob().readall())
             print("downloaded")
 
         
     except Exception as error:
         print("Error : ",error)
 
+
```

## Comparing `dopplrSDK-3.2.0.dist-info/LICENSE.txt` & `dopplrSDK-3.3.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

