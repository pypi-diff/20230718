# Comparing `tmp/zipline-cli-0.1.4.tar.gz` & `tmp/zipline-cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zipline-cli-0.1.4.tar", last modified: Thu Jul  6 21:06:56 2023, max compression
+gzip compressed data, was "zipline-cli-0.1.5.tar", last modified: Tue Jul 18 03:29:08 2023, max compression
```

## Comparing `zipline-cli-0.1.4.tar` & `zipline-cli-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 21:06:56.542989 zipline-cli-0.1.4/
--rw-rw-rw-   0        0        0     5049 2023-07-06 21:06:56.542989 zipline-cli-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4333 2023-07-05 23:27:06.000000 zipline-cli-0.1.4/README.md
--rw-rw-rw-   0        0        0      161 2023-07-06 21:06:56.543990 zipline-cli-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1153 2023-07-06 21:06:40.000000 zipline-cli-0.1.4/setup.py
--rw-rw-rw-   0        0        0     7885 2023-07-06 21:04:52.000000 zipline-cli-0.1.4/zipline.py
-drwxrwxrwx   0        0        0        0 2023-07-06 21:06:56.541988 zipline-cli-0.1.4/zipline_cli.egg-info/
--rw-rw-rw-   0        0        0     5049 2023-07-06 21:06:56.000000 zipline-cli-0.1.4/zipline_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-07-06 21:06:56.000000 zipline-cli-0.1.4/zipline_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 21:06:56.000000 zipline-cli-0.1.4/zipline_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-06 21:06:56.000000 zipline-cli-0.1.4/zipline_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-06 21:06:56.000000 zipline-cli-0.1.4/zipline_cli.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       39 2023-07-06 21:06:56.000000 zipline-cli-0.1.4/zipline_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-06 21:06:56.000000 zipline-cli-0.1.4/zipline_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 03:29:08.777843 zipline-cli-0.1.5/
+-rw-rw-rw-   0        0        0     5375 2023-07-18 03:29:08.777843 zipline-cli-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4655 2023-07-18 03:03:58.000000 zipline-cli-0.1.5/README.md
+-rw-rw-rw-   0        0        0      161 2023-07-18 03:29:08.778844 zipline-cli-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1153 2023-07-18 02:52:50.000000 zipline-cli-0.1.5/setup.py
+-rw-rw-rw-   0        0        0     7918 2023-07-18 02:58:25.000000 zipline-cli-0.1.5/zipline.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:29:08.777342 zipline-cli-0.1.5/zipline_cli.egg-info/
+-rw-rw-rw-   0        0        0     5375 2023-07-18 03:29:08.000000 zipline-cli-0.1.5/zipline_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-07-18 03:29:08.000000 zipline-cli-0.1.5/zipline_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 03:29:08.000000 zipline-cli-0.1.5/zipline_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-18 03:29:08.000000 zipline-cli-0.1.5/zipline_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 03:29:08.000000 zipline-cli-0.1.5/zipline_cli.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       39 2023-07-18 03:29:08.000000 zipline-cli-0.1.5/zipline_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-18 03:29:08.000000 zipline-cli-0.1.5/zipline_cli.egg-info/top_level.txt
```

### Comparing `zipline-cli-0.1.4/PKG-INFO` & `zipline-cli-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python 3 CLI for Zipline
 Home-page: https://github.com/cssnr/zipline-cli
 Author: Shane
 Author-email: shane@sapps.me
 Project-URL: Source, https://github.com/cssnr/zipline-cli
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -15,14 +15,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 [![Discord](https://img.shields.io/discord/899171661457293343?logo=discord&logoColor=white&label=Discord)](https://discord.gg/wXy6m2X8wY)
 [![PyPI](https://img.shields.io/github/issues-raw/cssnr/zipline-cli?logo=github&logoColor=white&label=Issues)](https://github.com/cssnr/zipline-cli/issues)
 [![Codacy Badge](https://img.shields.io/codacy/grade/1eee626c47fa4e6fb8b1ed3efdd3e518?logo=codacy&logoColor=white&label=Codacy)](https://app.codacy.com/gh/cssnr/zipline-cli/dashboard)
 [![PyPI](https://img.shields.io/pypi/v/zipline-cli?logo=python&logoColor=white&label=PyPi)](https://pypi.org/project/zipline-cli/)
+[![Build Status](https://drone.hosted-domains.com/api/badges/cssnr/zipline-cli/status.svg)](https://drone.hosted-domains.com/cssnr/zipline-cli)
 [![](https://repository-images.githubusercontent.com/661201286/8dfadbc8-94c0-4eaa-88bd-7ee351859510)](https://github.com/cssnr/zipline-cli)
 # Zipline CLI
 
 Python 3 CLI Uploader for Zipline.
 Zipline CLI is currently functional and **Under Active Development**.  
 Please open a [Feature Request](https://github.com/cssnr/zipline-cli/discussions/new?category=feature-requests)
 for new features and submit an [Issue](https://github.com/cssnr/zipline-cli/issues)
@@ -108,20 +109,23 @@
 
 ## Environment Variables
 
 Environment Variables are stored in the `.zipline` file in your home directory.
 
 *   Location: `~/.zipline` or `$HOME/.zipline`
 
-| Variable       | Description                                                                 |
-|----------------|-----------------------------------------------------------------------------|
-| ZIPLINE_URL    | URL to your Zipline Instance                                                |
-| ZIPLINE_TOKEN  | Authorization Token from Zipline                                            |
-| ZIPLINE_EMBED  | Set this enable Embed on your uploads                                       |
-| ZIPLINE_EXPIRE | See: https://zipline.diced.tech/docs/guides/upload-options#image-expiration |
+| Variable       | Description                                                                  |
+|----------------|------------------------------------------------------------------------------|
+| ZIPLINE_URL    | URL to your Zipline Instance                                                 |
+| ZIPLINE_TOKEN  | Authorization Token from Zipline                                             |
+| ZIPLINE_EMBED  | Set this enable Embed on your uploads                                        |
+| ZIPLINE_FORMAT | Output Format after upload. Variables: `{filename}`, `{url}` and `{raw_url}` |
+| ZIPLINE_EXPIRE | See: https://zipline.diced.tech/docs/guides/upload-options#image-expiration  |
+
+See [.zipline.example](.zipline.example) for an example `.zipline` file.
 
 You may override them by exporting the variables in your current environment
 or using the corresponding command line arguments. See `-h` for more info.
 
 ## Python API Reference
 
 Initialize the class with your Zipline URL.
```

### Comparing `zipline-cli-0.1.4/README.md` & `zipline-cli-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [![Discord](https://img.shields.io/discord/899171661457293343?logo=discord&logoColor=white&label=Discord)](https://discord.gg/wXy6m2X8wY)
 [![PyPI](https://img.shields.io/github/issues-raw/cssnr/zipline-cli?logo=github&logoColor=white&label=Issues)](https://github.com/cssnr/zipline-cli/issues)
 [![Codacy Badge](https://img.shields.io/codacy/grade/1eee626c47fa4e6fb8b1ed3efdd3e518?logo=codacy&logoColor=white&label=Codacy)](https://app.codacy.com/gh/cssnr/zipline-cli/dashboard)
 [![PyPI](https://img.shields.io/pypi/v/zipline-cli?logo=python&logoColor=white&label=PyPi)](https://pypi.org/project/zipline-cli/)
+[![Build Status](https://drone.hosted-domains.com/api/badges/cssnr/zipline-cli/status.svg)](https://drone.hosted-domains.com/cssnr/zipline-cli)
 [![](https://repository-images.githubusercontent.com/661201286/8dfadbc8-94c0-4eaa-88bd-7ee351859510)](https://github.com/cssnr/zipline-cli)
 # Zipline CLI
 
 Python 3 CLI Uploader for Zipline.
 Zipline CLI is currently functional and **Under Active Development**.  
 Please open a [Feature Request](https://github.com/cssnr/zipline-cli/discussions/new?category=feature-requests)
 for new features and submit an [Issue](https://github.com/cssnr/zipline-cli/issues)
@@ -91,20 +92,23 @@
 
 ## Environment Variables
 
 Environment Variables are stored in the `.zipline` file in your home directory.
 
 *   Location: `~/.zipline` or `$HOME/.zipline`
 
-| Variable       | Description                                                                 |
-|----------------|-----------------------------------------------------------------------------|
-| ZIPLINE_URL    | URL to your Zipline Instance                                                |
-| ZIPLINE_TOKEN  | Authorization Token from Zipline                                            |
-| ZIPLINE_EMBED  | Set this enable Embed on your uploads                                       |
-| ZIPLINE_EXPIRE | See: https://zipline.diced.tech/docs/guides/upload-options#image-expiration |
+| Variable       | Description                                                                  |
+|----------------|------------------------------------------------------------------------------|
+| ZIPLINE_URL    | URL to your Zipline Instance                                                 |
+| ZIPLINE_TOKEN  | Authorization Token from Zipline                                             |
+| ZIPLINE_EMBED  | Set this enable Embed on your uploads                                        |
+| ZIPLINE_FORMAT | Output Format after upload. Variables: `{filename}`, `{url}` and `{raw_url}` |
+| ZIPLINE_EXPIRE | See: https://zipline.diced.tech/docs/guides/upload-options#image-expiration  |
+
+See [.zipline.example](.zipline.example) for an example `.zipline` file.
 
 You may override them by exporting the variables in your current environment
 or using the corresponding command line arguments. See `-h` for more info.
 
 ## Python API Reference
 
 Initialize the class with your Zipline URL.
```

### Comparing `zipline-cli-0.1.4/setup.py` & `zipline-cli-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setup(
-    version='0.1.4',
+    version='0.1.5',
     name='zipline-cli',
     description='Python 3 CLI for Zipline',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/cssnr/zipline-cli',
     author='Shane',
     author_email='shane@sapps.me',
```

### Comparing `zipline-cli-0.1.4/zipline.py` & `zipline-cli-0.1.5/zipline.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 
 class ZipURL(object):
     """
     Zipline URL Object
     :param file_url: str: Zipline File Display URL
     """
-
     __slots__ = ['url', 'raw']
 
     def __init__(self, file_url: str):
         self.url: str = file_url
         self.raw: str = self._get_raw(file_url)
 
     def __repr__(self):
@@ -72,27 +71,25 @@
         """
         url = self.base_url + '/api/upload'
         files = {'file': (file_name, file_object)}
         headers = self._headers | overrides if overrides else self._headers
         r = requests.post(url, headers=headers, files=files)
         r.raise_for_status()
         return ZipURL(r.json()['files'][0])
-        # return f'https://example.com/dummy/{file_name}'
 
 
 def format_output(filename: str, url: ZipURL) -> str:
     """
     Format URL Output
     :param filename: str: Original or File Name
     :param url: ZipURL: ZipURL to Format
     :return: str: Formatted Output
     """
-    if url.raw:
-        return f'{filename}\n{url}\n{url.raw}'
-    return f'{filename}\n{url}'
+    zipline_format = config('ZIPLINE_FORMAT', '{filename}\n{url}\n{raw_url}')
+    return zipline_format.format(filename=filename, url=url, raw_url=url.raw)
 
 
 def gen_rand(length: Optional[int] = 4) -> str:
     """
     Generate Random Streng at Given length
     :param length: int: Length of Random String
     :return: str: Random String
@@ -139,15 +136,15 @@
             output += f'ZIPLINE_EXPIRE={expire}\n'
     with open(env_file, 'w') as f:
         f.write(output)
     print(f'Setup Complete. Variables Saved to: {env_file}')
     sys.exit(0)
 
 
-def main() -> None:
+def run() -> None:
     zipline_file = '.zipline'
     env_file = Path(os.path.expanduser('~')) / zipline_file
     dotenv_path = env_file if os.path.isfile(env_file) else find_dotenv(filename=zipline_file)
     env = load_dotenv(dotenv_path=dotenv_path)
 
     parser = argparse.ArgumentParser(description='Zipline CLI.')
     parser.add_argument('files', metavar='Files', type=str, nargs='*', help='Files to Upload.')
@@ -208,15 +205,19 @@
             # url: str = zipline.send_file(name, f)
             url: ZipURL = zipline.send_file(name, f)
             print(format_output(name, url))
             exit_code = 0
     sys.exit(exit_code)
 
 
-if __name__ == '__main__':
+def main() -> None:
     try:
-        main()
+        run()
     except KeyboardInterrupt:
         sys.exit(1)
     except Exception as error:
         print('\nError: {}'.format(str(error)))
         sys.exit(1)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `zipline-cli-0.1.4/zipline_cli.egg-info/PKG-INFO` & `zipline-cli-0.1.5/zipline_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python 3 CLI for Zipline
 Home-page: https://github.com/cssnr/zipline-cli
 Author: Shane
 Author-email: shane@sapps.me
 Project-URL: Source, https://github.com/cssnr/zipline-cli
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -15,14 +15,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 [![Discord](https://img.shields.io/discord/899171661457293343?logo=discord&logoColor=white&label=Discord)](https://discord.gg/wXy6m2X8wY)
 [![PyPI](https://img.shields.io/github/issues-raw/cssnr/zipline-cli?logo=github&logoColor=white&label=Issues)](https://github.com/cssnr/zipline-cli/issues)
 [![Codacy Badge](https://img.shields.io/codacy/grade/1eee626c47fa4e6fb8b1ed3efdd3e518?logo=codacy&logoColor=white&label=Codacy)](https://app.codacy.com/gh/cssnr/zipline-cli/dashboard)
 [![PyPI](https://img.shields.io/pypi/v/zipline-cli?logo=python&logoColor=white&label=PyPi)](https://pypi.org/project/zipline-cli/)
+[![Build Status](https://drone.hosted-domains.com/api/badges/cssnr/zipline-cli/status.svg)](https://drone.hosted-domains.com/cssnr/zipline-cli)
 [![](https://repository-images.githubusercontent.com/661201286/8dfadbc8-94c0-4eaa-88bd-7ee351859510)](https://github.com/cssnr/zipline-cli)
 # Zipline CLI
 
 Python 3 CLI Uploader for Zipline.
 Zipline CLI is currently functional and **Under Active Development**.  
 Please open a [Feature Request](https://github.com/cssnr/zipline-cli/discussions/new?category=feature-requests)
 for new features and submit an [Issue](https://github.com/cssnr/zipline-cli/issues)
@@ -108,20 +109,23 @@
 
 ## Environment Variables
 
 Environment Variables are stored in the `.zipline` file in your home directory.
 
 *   Location: `~/.zipline` or `$HOME/.zipline`
 
-| Variable       | Description                                                                 |
-|----------------|-----------------------------------------------------------------------------|
-| ZIPLINE_URL    | URL to your Zipline Instance                                                |
-| ZIPLINE_TOKEN  | Authorization Token from Zipline                                            |
-| ZIPLINE_EMBED  | Set this enable Embed on your uploads                                       |
-| ZIPLINE_EXPIRE | See: https://zipline.diced.tech/docs/guides/upload-options#image-expiration |
+| Variable       | Description                                                                  |
+|----------------|------------------------------------------------------------------------------|
+| ZIPLINE_URL    | URL to your Zipline Instance                                                 |
+| ZIPLINE_TOKEN  | Authorization Token from Zipline                                             |
+| ZIPLINE_EMBED  | Set this enable Embed on your uploads                                        |
+| ZIPLINE_FORMAT | Output Format after upload. Variables: `{filename}`, `{url}` and `{raw_url}` |
+| ZIPLINE_EXPIRE | See: https://zipline.diced.tech/docs/guides/upload-options#image-expiration  |
+
+See [.zipline.example](.zipline.example) for an example `.zipline` file.
 
 You may override them by exporting the variables in your current environment
 or using the corresponding command line arguments. See `-h` for more info.
 
 ## Python API Reference
 
 Initialize the class with your Zipline URL.
```

