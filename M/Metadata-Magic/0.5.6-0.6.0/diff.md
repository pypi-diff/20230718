# Comparing `tmp/Metadata_Magic-0.5.6-py3-none-any.whl.zip` & `tmp/Metadata_Magic-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,18 @@
-Zip file size: 83404 bytes, number of entries: 47
+Zip file size: 88076 bytes, number of entries: 51
 -rw-r--r--  2.0 unx       23 b- defN 23-Jul-09 20:05 metadata_magic/__init__.py
 -rw-r--r--  2.0 unx       23 b- defN 23-Jul-09 20:05 metadata_magic/main/__init__.py
 -rw-r--r--  2.0 unx     3095 b- defN 23-Jul-16 21:31 metadata_magic/main/meta_finder.py
 -rw-r--r--  2.0 unx    12155 b- defN 23-Jul-16 19:18 metadata_magic/main/meta_reader.py
 -rw-r--r--  2.0 unx       23 b- defN 23-Jul-09 20:05 metadata_magic/main/comic_archive/__init__.py
--rw-r--r--  2.0 unx    13676 b- defN 23-Jul-17 17:48 metadata_magic/main/comic_archive/comic_archive.py
+-rw-r--r--  2.0 unx     2846 b- defN 23-Jul-18 17:48 metadata_magic/main/comic_archive/archive_all.py
+-rw-r--r--  2.0 unx    13954 b- defN 23-Jul-17 21:24 metadata_magic/main/comic_archive/comic_archive.py
 -rw-r--r--  2.0 unx     5838 b- defN 23-Jul-16 22:49 metadata_magic/main/comic_archive/comic_archive_update.py
 -rw-r--r--  2.0 unx     9738 b- defN 23-Jul-16 19:18 metadata_magic/main/comic_archive/comic_xml.py
+-rw-r--r--  2.0 unx     3198 b- defN 23-Jul-18 17:56 metadata_magic/main/comic_archive/extract_all.py
 -rw-r--r--  2.0 unx     7923 b- defN 23-Jul-16 19:18 metadata_magic/main/comic_archive/series_info.py
 -rw-r--r--  2.0 unx       23 b- defN 23-Jul-09 20:05 metadata_magic/main/epub/__init__.py
 -rw-r--r--  2.0 unx    33790 b- defN 23-Jul-16 19:18 metadata_magic/main/epub/epub.py
 -rw-r--r--  2.0 unx       23 b- defN 23-Jul-09 20:05 metadata_magic/main/error_finding/__init__.py
 -rw-r--r--  2.0 unx     6038 b- defN 23-Jul-17 19:47 metadata_magic/main/error_finding/missing_fields.py
 -rw-r--r--  2.0 unx     2076 b- defN 23-Jul-16 19:18 metadata_magic/main/error_finding/missing_media.py
 -rw-r--r--  2.0 unx     2098 b- defN 23-Jul-16 19:18 metadata_magic/main/error_finding/missing_metadata.py
@@ -20,30 +22,32 @@
 -rw-r--r--  2.0 unx     6412 b- defN 23-Jul-16 20:51 metadata_magic/main/rename/meta_rename.py
 -rw-r--r--  2.0 unx     7700 b- defN 23-Jul-16 19:18 metadata_magic/main/rename/rename_tools.py
 -rw-r--r--  2.0 unx     4400 b- defN 23-Jul-16 19:18 metadata_magic/main/rename/sort_rename.py
 -rw-r--r--  2.0 unx       23 b- defN 23-Jul-09 20:05 metadata_magic/test/__init__.py
 -rw-r--r--  2.0 unx     4267 b- defN 23-Jul-16 19:18 metadata_magic/test/test_meta_finder.py
 -rw-r--r--  2.0 unx    22953 b- defN 23-Jul-16 19:18 metadata_magic/test/test_meta_reader.py
 -rw-r--r--  2.0 unx       23 b- defN 23-Jul-09 20:05 metadata_magic/test/comic_archive/__init__.py
--rw-r--r--  2.0 unx    12249 b- defN 23-Jul-17 17:48 metadata_magic/test/comic_archive/test_comic_archive.py
--rw-r--r--  2.0 unx     5322 b- defN 23-Jul-16 22:19 metadata_magic/test/comic_archive/test_comic_archive_update.py
+-rw-r--r--  2.0 unx     3060 b- defN 23-Jul-17 21:27 metadata_magic/test/comic_archive/test_archive_all.py
+-rw-r--r--  2.0 unx    13189 b- defN 23-Jul-17 21:22 metadata_magic/test/comic_archive/test_comic_archive.py
+-rw-r--r--  2.0 unx     5322 b- defN 23-Jul-17 20:48 metadata_magic/test/comic_archive/test_comic_archive_update.py
 -rw-r--r--  2.0 unx    19952 b- defN 23-Jul-16 19:18 metadata_magic/test/comic_archive/test_comic_xml.py
+-rw-r--r--  2.0 unx     4941 b- defN 23-Jul-18 17:43 metadata_magic/test/comic_archive/test_extract_all.py
 -rw-r--r--  2.0 unx     8700 b- defN 23-Jul-16 19:18 metadata_magic/test/comic_archive/test_series_info.py
 -rw-r--r--  2.0 unx       23 b- defN 23-Jul-09 20:05 metadata_magic/test/epub/__init__.py
 -rw-r--r--  2.0 unx    43439 b- defN 23-Jul-16 19:18 metadata_magic/test/epub/test_epub.py
 -rw-r--r--  2.0 unx       23 b- defN 23-Jul-09 20:05 metadata_magic/test/error_finding/__init__.py
 -rw-r--r--  2.0 unx     7041 b- defN 23-Jul-17 19:12 metadata_magic/test/error_finding/test_missing_fields.py
 -rw-r--r--  2.0 unx     1539 b- defN 23-Jul-16 19:18 metadata_magic/test/error_finding/test_missing_media.py
 -rw-r--r--  2.0 unx     1580 b- defN 23-Jul-16 19:18 metadata_magic/test/error_finding/test_missing_metadata.py
 -rw-r--r--  2.0 unx       23 b- defN 23-Jul-09 20:05 metadata_magic/test/file_tools/__init__.py
 -rw-r--r--  2.0 unx    15775 b- defN 23-Jul-17 16:58 metadata_magic/test/file_tools/test_file_tools.py
 -rw-r--r--  2.0 unx       23 b- defN 23-Jul-09 20:05 metadata_magic/test/rename/__init__.py
 -rw-r--r--  2.0 unx     9707 b- defN 23-Jul-16 19:18 metadata_magic/test/rename/test_meta_rename.py
 -rw-r--r--  2.0 unx     9157 b- defN 23-Jul-16 19:18 metadata_magic/test/rename/test_rename_tools.py
 -rw-r--r--  2.0 unx     6745 b- defN 23-Jul-16 19:18 metadata_magic/test/rename/test_sort_rename.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jul-17 19:47 Metadata_Magic-0.5.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     5754 b- defN 23-Jul-17 19:47 Metadata_Magic-0.5.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 19:47 Metadata_Magic-0.5.6.dist-info/WHEEL
--rw-r--r--  2.0 unx      634 b- defN 23-Jul-17 19:47 Metadata_Magic-0.5.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 23-Jul-17 19:47 Metadata_Magic-0.5.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4661 b- defN 23-Jul-17 19:47 Metadata_Magic-0.5.6.dist-info/RECORD
-47 files, 340517 bytes uncompressed, 75696 bytes compressed:  77.8%
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-18 18:04 Metadata_Magic-0.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5754 b- defN 23-Jul-18 18:04 Metadata_Magic-0.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-18 18:04 Metadata_Magic-0.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      779 b- defN 23-Jul-18 18:04 Metadata_Magic-0.6.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-18 18:04 Metadata_Magic-0.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5091 b- defN 23-Jul-18 18:04 Metadata_Magic-0.6.0.dist-info/RECORD
+51 files, 356355 bytes uncompressed, 79660 bytes compressed:  77.6%
```

## zipnote {}

```diff
@@ -9,23 +9,29 @@
 
 Filename: metadata_magic/main/meta_reader.py
 Comment: 
 
 Filename: metadata_magic/main/comic_archive/__init__.py
 Comment: 
 
+Filename: metadata_magic/main/comic_archive/archive_all.py
+Comment: 
+
 Filename: metadata_magic/main/comic_archive/comic_archive.py
 Comment: 
 
 Filename: metadata_magic/main/comic_archive/comic_archive_update.py
 Comment: 
 
 Filename: metadata_magic/main/comic_archive/comic_xml.py
 Comment: 
 
+Filename: metadata_magic/main/comic_archive/extract_all.py
+Comment: 
+
 Filename: metadata_magic/main/comic_archive/series_info.py
 Comment: 
 
 Filename: metadata_magic/main/epub/__init__.py
 Comment: 
 
 Filename: metadata_magic/main/epub/epub.py
@@ -69,23 +75,29 @@
 
 Filename: metadata_magic/test/test_meta_reader.py
 Comment: 
 
 Filename: metadata_magic/test/comic_archive/__init__.py
 Comment: 
 
+Filename: metadata_magic/test/comic_archive/test_archive_all.py
+Comment: 
+
 Filename: metadata_magic/test/comic_archive/test_comic_archive.py
 Comment: 
 
 Filename: metadata_magic/test/comic_archive/test_comic_archive_update.py
 Comment: 
 
 Filename: metadata_magic/test/comic_archive/test_comic_xml.py
 Comment: 
 
+Filename: metadata_magic/test/comic_archive/test_extract_all.py
+Comment: 
+
 Filename: metadata_magic/test/comic_archive/test_series_info.py
 Comment: 
 
 Filename: metadata_magic/test/epub/__init__.py
 Comment: 
 
 Filename: metadata_magic/test/epub/test_epub.py
@@ -117,26 +129,26 @@
 
 Filename: metadata_magic/test/rename/test_rename_tools.py
 Comment: 
 
 Filename: metadata_magic/test/rename/test_sort_rename.py
 Comment: 
 
-Filename: Metadata_Magic-0.5.6.dist-info/LICENSE
+Filename: Metadata_Magic-0.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: Metadata_Magic-0.5.6.dist-info/METADATA
+Filename: Metadata_Magic-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: Metadata_Magic-0.5.6.dist-info/WHEEL
+Filename: Metadata_Magic-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: Metadata_Magic-0.5.6.dist-info/entry_points.txt
+Filename: Metadata_Magic-0.6.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: Metadata_Magic-0.5.6.dist-info/top_level.txt
+Filename: Metadata_Magic-0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: Metadata_Magic-0.5.6.dist-info/RECORD
+Filename: Metadata_Magic-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## metadata_magic/main/comic_archive/comic_archive.py

```diff
@@ -40,15 +40,15 @@
     # Return None if directory is empty
     full_directory = abspath(directory)
     if len(listdir(full_directory)) == 0:
         return None
     # Create CBZ filename
     filename = basename(full_directory) + ".cbz"
     if name is not None:
-        filename = f"{name}.cbz"
+        filename = create_filename(name) + ".cbz"
     cbz_file = abspath(join(full_directory, filename))
     # Update CBZ if it already exists
     if exists(cbz_file):
         if metadata is not None:
             update_cbz_info(cbz_file, metadata)
         return cbz_file
     # Check if there are existing directories
@@ -57,15 +57,21 @@
     for file in files:
         if isdir(abspath(join(full_directory, file))):
             move_files = False
             break
     # Move files if required
     if move_files:
         # Create new folder to contain files
-        folder_name = files[0][:len(files[0]) - len(get_extension(files[0]))]
+        folder_name = name
+        if folder_name is None:
+            try:
+                folder_name = metadata["title"]
+                assert folder_name is not None
+            except (AssertionError, KeyError, TypeError):
+                folder_name = files[0][:len(files[0]) - len(get_extension(files[0]))]
         folder_name = get_available_filename("AAAAAAAAAA", create_filename(folder_name), full_directory)
         new_folder = abspath(join(full_directory, folder_name))
         mkdir(new_folder)
         # Move existing files to the new folder
         for file in files:
             current_file = abspath(join(full_directory, file))
             new_file = abspath(join(new_folder, file))
@@ -128,15 +134,15 @@
     if extract_zip(full_cbz_file, temp_dir):
         # Delete existing ComicInfo.xml files
         xml_files = find_files_of_type(temp_dir, ".xml")
         for xml_file in xml_files:
             if basename(xml_file) == "ComicInfo.xml":
                 remove(xml_file)
         # Pack files into archive using new metadata
-        new_cbz = create_cbz(temp_dir, metadata=metadata)
+        new_cbz = create_cbz(temp_dir, name=metadata["title"], metadata=metadata)
         # Replace the old cbz file
         remove(full_cbz_file)
         copy(new_cbz, full_cbz_file)
         remove(new_cbz)
     
 def create_comic_archive(path:str,
                 rp_description:bool=False,
```

## metadata_magic/test/comic_archive/test_comic_archive.py

```diff
@@ -88,26 +88,26 @@
     cbz_directory = get_temp_dir("dvk_cbz_test")
     text_file = abspath(join(cbz_directory, "new"))
     media_file = abspath(join(cbz_directory, "things.txt"))
     write_text_file(text_file, "NEWER")
     write_text_file(media_file, "More things")
     assert exists(text_file)
     assert exists(media_file)
-    cbz_file = create_cbz(cbz_directory, "None", metadata=metadata, remove_files=True)
-    assert listdir(cbz_directory) == ["None.cbz"]
+    cbz_file = create_cbz(cbz_directory, "new", metadata=metadata, remove_files=True)
+    assert listdir(cbz_directory) == ["new.cbz"]
     extract_directory = get_temp_dir("dvk_extract_test")
     assert extract_zip(cbz_file, extract_directory)
     assert sorted(listdir(extract_directory)) == ["ComicInfo.xml", "new-2"]
     sub_directory = abspath(join(extract_directory, "new-2"))
     assert sorted(listdir(sub_directory)) == ["new", "things.txt"]
     # Test that CBZ is only updated with new metadata if CBZ already exists
     metadata["title"] = "New!"
     metadata["tags"] = "Some, More, Stuff"
-    cbz_file = create_cbz(cbz_directory, "None", metadata=metadata)
-    assert listdir(cbz_directory) == ["None.cbz"]
+    cbz_file = create_cbz(cbz_directory, "new", metadata=metadata)
+    assert listdir(cbz_directory) == ["new.cbz"]
     extract_directory = get_temp_dir("dvk_extract_test")
     assert extract_zip(cbz_file, extract_directory)
     assert sorted(listdir(extract_directory)) == ["ComicInfo.xml", "new-2"]
     sub_directory = abspath(join(extract_directory, "new-2"))
     assert sorted(listdir(sub_directory)) == ["new", "things.txt"]
     read_meta = read_comic_info(abspath(join(extract_directory, "ComicInfo.xml")))
     assert read_meta["title"] == "New!"
@@ -182,15 +182,15 @@
     """
     Tests the update_cbz_info function.
     """
     # Create a test cbz file
     temp_dir = get_temp_dir()
     text_file = abspath(join(temp_dir, "other.txt"))
     metadata = get_empty_metadata()
-    metadata["title"] = "Old title."
+    metadata["title"] = "Old Title."
     metadata["tags"] = "Some,Tags"
     write_text_file(text_file, "This is text!")
     assert exists(text_file)
     cbz_file = create_cbz(temp_dir, metadata=metadata)
     assert exists(cbz_file)
     # Update cbz with new info
     metadata["title"] = "New Title!!!"
@@ -201,16 +201,16 @@
     assert read_meta["title"] == "New Title!!!"
     assert read_meta["artist"] == "Dude"
     assert read_meta["tags"] == "Something,Else"
     # Test that all other archived files are still present
     extract_dir = abspath(join(temp_dir, "ext"))
     mkdir(extract_dir)
     assert extract_zip(cbz_file, extract_dir)
-    assert sorted(listdir(extract_dir)) == ["ComicInfo.xml", "other"]
-    assert listdir(abspath(join(extract_dir, "other"))) == ["other.txt"]
+    assert sorted(listdir(extract_dir)) == ["ComicInfo.xml", "Old Title"]
+    assert listdir(abspath(join(extract_dir, "Old Title"))) == ["other.txt"]
     # Test updating cbz that had no comic info in the first place
     temp_dir = get_temp_dir()
     text_file = abspath(join(temp_dir, "text.txt"))
     other_file = abspath(join(temp_dir, "other.txt"))
     write_text_file(text_file, "This is text!")
     write_text_file(other_file, "More text!")
     assert exists(text_file)
@@ -263,7 +263,27 @@
     assert read_meta["description"] is None
     extract_dir = abspath(join(temp_dir, "extracted"))
     mkdir(extract_dir)
     assert extract_zip(cbz_file, extract_dir)
     assert sorted(listdir(extract_dir)) == ["ComicInfo.xml", "Internal", "Other.png"]
     sub_dir = abspath(join(extract_dir, "Internal"))
     assert listdir(sub_dir) == ["Thing.txt"]
+    # Test that updating adds the correctly named internal folder
+    temp_dir = get_temp_dir()
+    text_file = abspath(join(temp_dir, "text.txt"))
+    write_text_file(text_file, "text")
+    assert exists(text_file)
+    cbz_file = abspath(join(temp_dir, "internal.cbz"))
+    assert create_zip(temp_dir, cbz_file)
+    assert exists(cbz_file)
+    metadata["title"] = "Should Reflect Inside."
+    update_cbz_info(cbz_file, metadata)
+    read_meta = get_info_from_cbz(cbz_file)
+    assert read_meta["title"] == "Should Reflect Inside."
+    assert read_meta["artist"] == "New"
+    assert read_meta["description"] is None
+    extract_dir = abspath(join(temp_dir, "extracted"))
+    mkdir(extract_dir)
+    assert extract_zip(cbz_file, extract_dir)
+    assert sorted(listdir(extract_dir)) == ["ComicInfo.xml", "Should Reflect Inside"]
+    sub_dir = abspath(join(extract_dir, "Should Reflect Inside"))
+    assert listdir(sub_dir) == ["text.txt"]
```

## metadata_magic/test/comic_archive/test_comic_archive_update.py

```diff
@@ -31,81 +31,81 @@
     cbz_file_2 = abspath(join(temp_dir, "new.cbz"))
     cbz_file_3 = abspath(join(temp_dir, "other.cbz"))
     copy(cbz_file_1, cbz_file_2)
     copy(cbz_file_1, cbz_file_3)
     assert exists(cbz_file_1)
     assert exists(cbz_file_2)
     assert exists(cbz_file_3)
-    assert sorted(listdir(temp_dir)) == ["Name.cbz", "new.cbz", "other.cbz", "text"]
+    assert sorted(listdir(temp_dir)) == ["Name", "Name.cbz", "new.cbz", "other.cbz"]
     # Test updating publisher
     metadata = get_empty_metadata()
     metadata["publisher"] = "New Publisher"
     mass_update_cbzs(temp_dir, metadata)
     read_meta = get_info_from_cbz(cbz_file_1)
     assert read_meta["title"] == "This is a title!"
     assert read_meta["artist"] == "Person"
     assert read_meta["writer"] == "New"
     assert read_meta["cover_artist"] == "Cover"
     assert read_meta["publisher"] == "New Publisher"
     assert read_meta["age_rating"] == "Unknown"
-    assert sorted(listdir(temp_dir)) == ["Name.cbz", "new.cbz", "other.cbz", "text"]
+    assert sorted(listdir(temp_dir)) == ["Name", "Name.cbz", "new.cbz", "other.cbz"]
     # Test updating artists
     metadata = get_empty_metadata()
     metadata["artist"] = "New Guy"
     metadata["writer"] = "Writer Lad"
     metadata["cover_artist"] = "Other"
     mass_update_cbzs(temp_dir, metadata)
     read_meta = get_info_from_cbz(cbz_file_2)
     assert read_meta["title"] == "This is a title!"
     assert read_meta["artist"] == "New Guy"
     assert read_meta["writer"] == "Writer Lad"
     assert read_meta["cover_artist"] == "Other"
     assert read_meta["publisher"] == "New Publisher"
     assert read_meta["age_rating"] == "Unknown"
     assert read_meta["score"] == "3"
-    assert sorted(listdir(temp_dir)) == ["Name.cbz", "new.cbz", "other.cbz", "text"]
+    assert sorted(listdir(temp_dir)) == ["Name", "Name.cbz", "new.cbz", "other.cbz"]
     # Test updating age rating
     metadata = get_empty_metadata()
     metadata["age_rating"] = "Everyone"
     mass_update_cbzs(temp_dir, metadata)
     read_meta = get_info_from_cbz(cbz_file_3)
     assert read_meta["title"] == "This is a title!"
     assert read_meta["artist"] == "New Guy"
     assert read_meta["writer"] == "Writer Lad"
     assert read_meta["cover_artist"] == "Other"
     assert read_meta["publisher"] == "New Publisher"
     assert read_meta["age_rating"] == "Everyone"
     assert read_meta["score"] == "3"
-    assert sorted(listdir(temp_dir)) == ["Name.cbz", "new.cbz", "other.cbz", "text"]
+    assert sorted(listdir(temp_dir)) == ["Name", "Name.cbz", "new.cbz", "other.cbz"]
     # Test updating content rating
     metadata = get_empty_metadata()
     metadata["age_rating"] = "Everyone"
     mass_update_cbzs(temp_dir, metadata)
     read_meta = get_info_from_cbz(cbz_file_3)
     assert read_meta["title"] == "This is a title!"
     assert read_meta["artist"] == "New Guy"
     assert read_meta["writer"] == "Writer Lad"
     assert read_meta["cover_artist"] == "Other"
     assert read_meta["publisher"] == "New Publisher"
     assert read_meta["age_rating"] == "Everyone"
     assert read_meta["score"] == "3"
-    assert sorted(listdir(temp_dir)) == ["Name.cbz", "new.cbz", "other.cbz", "text"]
+    assert sorted(listdir(temp_dir)) == ["Name", "Name.cbz", "new.cbz", "other.cbz"]
     # Test updating score
     metadata = get_empty_metadata()
     metadata["score"] = 5
     mass_update_cbzs(temp_dir, metadata)
     read_meta = get_info_from_cbz(cbz_file_2)
     assert read_meta["title"] == "This is a title!"
     assert read_meta["artist"] == "New Guy"
     assert read_meta["writer"] == "Writer Lad"
     assert read_meta["cover_artist"] == "Other"
     assert read_meta["publisher"] == "New Publisher"
     assert read_meta["age_rating"] == "Everyone"
     assert read_meta["score"] == "5"
-    assert sorted(listdir(temp_dir)) == ["Name.cbz", "new.cbz", "other.cbz", "text"]
+    assert sorted(listdir(temp_dir)) == ["Name", "Name.cbz", "new.cbz", "other.cbz"]
     # Test updating multiple fields
     metadata = get_empty_metadata()
     metadata["title"] = "Blah"
     metadata["artist"] = "Madam Anonymous"
     metadata["writer"] = None
     metadata["publisher"] = "Blah Inc."
     metadata["score"] = None
@@ -114,8 +114,8 @@
     assert read_meta["title"] == "This is a title!"
     assert read_meta["artist"] == "Madam Anonymous"
     assert read_meta["writer"] == "Writer Lad"
     assert read_meta["cover_artist"] == "Other"
     assert read_meta["publisher"] == "Blah Inc."
     assert read_meta["age_rating"] == "Everyone"
     assert read_meta["score"] == "5"
-    assert sorted(listdir(temp_dir)) == ["Name.cbz", "new.cbz", "other.cbz", "text"]
+    assert sorted(listdir(temp_dir)) == ["Name", "Name.cbz", "new.cbz", "other.cbz"]
```

## Comparing `Metadata_Magic-0.5.6.dist-info/LICENSE` & `Metadata_Magic-0.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Metadata_Magic-0.5.6.dist-info/METADATA` & `Metadata_Magic-0.6.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Metadata-Magic
-Version: 0.5.6
+Version: 0.6.0
 Summary: Utility for managing metadata.
 Home-page: https://github.com/Drakovek/MetadataMagic
 Author: Drakovek
 Author-email: DrakovekMail@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

## Comparing `Metadata_Magic-0.5.6.dist-info/entry_points.txt` & `Metadata_Magic-0.6.0.dist-info/entry_points.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 [console_scripts]
+archive-all-comics = metadata_magic.main.comic_archive.archive_all:main
 archive-book = metadata_magic.main.epub.epub:main
 archive-comic = metadata_magic.main.comic_archive.comic_archive:main
-archive-comic-update = metadata_magic.main.comic_archive.comic_archive_update:main
 archive-series = metadata_magic.main.comic_archive.series_info:main
+extract-all-comics = metadata_magic.main.comic_archive.extract_all:main
 meta-missing-fields = metadata_magic.main.error_finding.missing_fields:main
 meta-missing-media = metadata_magic.main.error_finding.missing_media:main
 meta-missing-metadata = metadata_magic.main.error_finding.missing_metadata:main
 meta-rename = metadata_magic.main.rename.meta_rename:main
 sort-rename = metadata_magic.main.rename.sort_rename:main
+update-comic-archives = metadata_magic.main.comic_archive.comic_archive_update:main
```

## Comparing `Metadata_Magic-0.5.6.dist-info/RECORD` & `Metadata_Magic-0.6.0.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 metadata_magic/__init__.py,sha256=1oLL20yLB1GL9IbFiZD8OReDqiCpFr-yetIR6x1cNkI,23
 metadata_magic/main/__init__.py,sha256=1oLL20yLB1GL9IbFiZD8OReDqiCpFr-yetIR6x1cNkI,23
 metadata_magic/main/meta_finder.py,sha256=x-iI3TRCsvEsnRbR0EwL1anPsr6c6bG-cvHmymfo2rg,3095
 metadata_magic/main/meta_reader.py,sha256=g06oBVknecoPT4Gi7PYwz5QAwnilrjtOGfVcFzDiJvc,12155
 metadata_magic/main/comic_archive/__init__.py,sha256=1oLL20yLB1GL9IbFiZD8OReDqiCpFr-yetIR6x1cNkI,23
-metadata_magic/main/comic_archive/comic_archive.py,sha256=Z_Y9vNg_j6XBJ43ixybWfmO3P7pmyxcmTN5-kk2jSrI,13676
+metadata_magic/main/comic_archive/archive_all.py,sha256=QDuUq_HfIQsFsKB8KX_Xronl_LIhQHoyG7aZgILvwS8,2846
+metadata_magic/main/comic_archive/comic_archive.py,sha256=qLIMeqTAthrEDb8hkwRKi6Ho9JZGxU6pE_uBVEQ1y98,13954
 metadata_magic/main/comic_archive/comic_archive_update.py,sha256=cBmBtykff84DIIw0m8kSXfwbFIFI4sIq8LuBo99ago0,5838
 metadata_magic/main/comic_archive/comic_xml.py,sha256=BKDtctPb5qoNE_bcnFYCB0lz1bhxvaroftxyuZWDO3k,9738
+metadata_magic/main/comic_archive/extract_all.py,sha256=cljI9G3FAHPAERrhJtILClJRTIdR6H-ii22r5VqaxY0,3198
 metadata_magic/main/comic_archive/series_info.py,sha256=IiUl2sLBswXyV8gCDzHVM5SlnPhhOen-GHTrd_FhTGs,7923
 metadata_magic/main/epub/__init__.py,sha256=1oLL20yLB1GL9IbFiZD8OReDqiCpFr-yetIR6x1cNkI,23
 metadata_magic/main/epub/epub.py,sha256=88kP4pfHbRKnTuy1wmExsygWYnB4w77ER-vP-ToOc3E,33790
 metadata_magic/main/error_finding/__init__.py,sha256=1oLL20yLB1GL9IbFiZD8OReDqiCpFr-yetIR6x1cNkI,23
 metadata_magic/main/error_finding/missing_fields.py,sha256=jrmtwGPiR-2wectIulqAaETQg0b01XkPLE23DAd5ctc,6038
 metadata_magic/main/error_finding/missing_media.py,sha256=sstDLfPna9x2GtGWkqHdFhNdrS0AVUHNLzUrC5XbfOU,2076
 metadata_magic/main/error_finding/missing_metadata.py,sha256=-dLlvVQ4TTw7Sm5N_g4_t1sMPh_UBVF7prxb1hBAICY,2098
@@ -19,29 +21,31 @@
 metadata_magic/main/rename/meta_rename.py,sha256=Q-H0lygLdFLxxrp2Rt1KPLrQjN-xUhB4JLS-zcXBfgE,6412
 metadata_magic/main/rename/rename_tools.py,sha256=00yAAG4FFaApfuh7dIp0GPzABdnKW5bahlNeOyZM1wI,7700
 metadata_magic/main/rename/sort_rename.py,sha256=AFoh87qy9oG4y2lTjb6vwGIftZbyLz_eKDU0PwAjujo,4400
 metadata_magic/test/__init__.py,sha256=1oLL20yLB1GL9IbFiZD8OReDqiCpFr-yetIR6x1cNkI,23
 metadata_magic/test/test_meta_finder.py,sha256=4ixgPHJcILa7uX8DuMoSa1GodDG2UuCKqlZdf_3gQbc,4267
 metadata_magic/test/test_meta_reader.py,sha256=6wwbET3mD5CS5BC48CVrLswztr-BMuZBIEe1hU9KW88,22953
 metadata_magic/test/comic_archive/__init__.py,sha256=1oLL20yLB1GL9IbFiZD8OReDqiCpFr-yetIR6x1cNkI,23
-metadata_magic/test/comic_archive/test_comic_archive.py,sha256=_ZoIEfNagSvh88i4yZkVuzeQlm3ofaVyhnsshdaL_DY,12249
-metadata_magic/test/comic_archive/test_comic_archive_update.py,sha256=svayU6tiuRc5e24FIj-HpmYaYncU0igtuXXa5fYH6sk,5322
+metadata_magic/test/comic_archive/test_archive_all.py,sha256=vfuYIJezEgcXRbVk6Gn5kjH_pvbux6AZbxRF7aw-t6U,3060
+metadata_magic/test/comic_archive/test_comic_archive.py,sha256=bNsgxH0PYfZcSSzq9nO6GetHuDbgqOEOjss8InZberg,13189
+metadata_magic/test/comic_archive/test_comic_archive_update.py,sha256=XHJN678n-vZYtRWSdsrt5HJRVa-APeHBwW66wHZ-Jxw,5322
 metadata_magic/test/comic_archive/test_comic_xml.py,sha256=RGFNnNG-Vt1vQ2COH31SHIVjIFoCVpdFKgz5Ytqq1Ws,19952
+metadata_magic/test/comic_archive/test_extract_all.py,sha256=e_jOzHGgODyf-Q_-6YC8vOyonnfSDpVgjqi5GtHM-HA,4941
 metadata_magic/test/comic_archive/test_series_info.py,sha256=HXRNgPZDlfMAVHfq2nYRJ61JxJctgV0Z_jIG6NrVffk,8700
 metadata_magic/test/epub/__init__.py,sha256=1oLL20yLB1GL9IbFiZD8OReDqiCpFr-yetIR6x1cNkI,23
 metadata_magic/test/epub/test_epub.py,sha256=NzxqUgqBhFvou4M67xy-oFBPOCtNxYyZi5Y5pYf2r_A,43439
 metadata_magic/test/error_finding/__init__.py,sha256=1oLL20yLB1GL9IbFiZD8OReDqiCpFr-yetIR6x1cNkI,23
 metadata_magic/test/error_finding/test_missing_fields.py,sha256=1qiQO2bv2fJcXpWPCztYpqH29-MfPiafF57T5nuUc9E,7041
 metadata_magic/test/error_finding/test_missing_media.py,sha256=geB0qFLWu0aQPbN7J6cmMtRoTckQBS14jP1lWMz2GbU,1539
 metadata_magic/test/error_finding/test_missing_metadata.py,sha256=Se7zfcypO-7wJRePdIbzXvDROF6C1Du2s0vGD1xz648,1580
 metadata_magic/test/file_tools/__init__.py,sha256=1oLL20yLB1GL9IbFiZD8OReDqiCpFr-yetIR6x1cNkI,23
 metadata_magic/test/file_tools/test_file_tools.py,sha256=2GtU_jowSlJx7FW8bg8shwA6ZZCc08ziB1xHwrjbrTE,15775
 metadata_magic/test/rename/__init__.py,sha256=1oLL20yLB1GL9IbFiZD8OReDqiCpFr-yetIR6x1cNkI,23
 metadata_magic/test/rename/test_meta_rename.py,sha256=X2S6iBmwW-xaI3sc_0xjf_ft4TBT4swhOKC8O1v07yI,9707
 metadata_magic/test/rename/test_rename_tools.py,sha256=3gZN0TEmt5GKj31RII1ZTw4fJBX2hPx0caiTSClHk6c,9157
 metadata_magic/test/rename/test_sort_rename.py,sha256=L8_9Mm2SeUQ1VuOIrpsXpj0NVOIttrLkXmVx-xGWmiM,6745
-Metadata_Magic-0.5.6.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-Metadata_Magic-0.5.6.dist-info/METADATA,sha256=eEjB1oEtmCS72Uouh58HTs5Rqi3T3bTNBdziVdsk8S8,5754
-Metadata_Magic-0.5.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-Metadata_Magic-0.5.6.dist-info/entry_points.txt,sha256=jPL5jXbyJTcZl-M7wzvduFvv9Vyx3lFtIUUpzp85MB4,634
-Metadata_Magic-0.5.6.dist-info/top_level.txt,sha256=xiXw1Za6sizhihwckAr1UAU5GxhrzpKEd6cIPCRmuT0,15
-Metadata_Magic-0.5.6.dist-info/RECORD,,
+Metadata_Magic-0.6.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+Metadata_Magic-0.6.0.dist-info/METADATA,sha256=tD0VYumSzZXUjY3qDyEl_qhAwVqv64wnVb4LLHmHCHk,5754
+Metadata_Magic-0.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+Metadata_Magic-0.6.0.dist-info/entry_points.txt,sha256=3tavBkM0cW3cnLKx8f-Nyy98b8NnQqILUifCjVUQw8M,779
+Metadata_Magic-0.6.0.dist-info/top_level.txt,sha256=xiXw1Za6sizhihwckAr1UAU5GxhrzpKEd6cIPCRmuT0,15
+Metadata_Magic-0.6.0.dist-info/RECORD,,
```

