# Comparing `tmp/UnityPy-1.9.8.tar.gz` & `tmp/UnityPy-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnityPy-1.9.8.tar", last modified: Wed Aug  3 16:40:40 2022, max compression
+gzip compressed data, was "UnityPy-1.9.9.tar", last modified: Thu Aug  4 09:36:45 2022, max compression
```

## Comparing `UnityPy-1.9.8.tar` & `UnityPy-1.9.9.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-03 16:40:40.155273 UnityPy-1.9.8/
--rw-r--r--   0 runner     (501) staff       (20)     1067 2022-08-03 16:39:04.000000 UnityPy-1.9.8/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)    12682 2022-08-03 16:40:40.155463 UnityPy-1.9.8/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    11652 2022-08-03 16:39:04.000000 UnityPy-1.9.8/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-03 16:40:40.097164 UnityPy-1.9.8/UnityPy/
--rw-r--r--   0 runner     (501) staff       (20)      164 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-03 16:40:40.119233 UnityPy-1.9.8/UnityPy/classes/
--rw-r--r--   0 runner     (501) staff       (20)      315 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/Animation.py
--rw-r--r--   0 runner     (501) staff       (20)    20197 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/AnimationClip.py
--rw-r--r--   0 runner     (501) staff       (20)     1352 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/Animator.py
--rw-r--r--   0 runner     (501) staff       (20)    10915 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/AnimatorController.py
--rw-r--r--   0 runner     (501) staff       (20)      553 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/AnimatorOverrideController.py
--rw-r--r--   0 runner     (501) staff       (20)      769 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/AssetBundle.py
--rw-r--r--   0 runner     (501) staff       (20)     2520 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/AudioClip.py
--rw-r--r--   0 runner     (501) staff       (20)     5045 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/Avatar.py
--rw-r--r--   0 runner     (501) staff       (20)      575 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/Behaviour.py
--rw-r--r--   0 runner     (501) staff       (20)      448 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/BuildSettings.py
--rw-r--r--   0 runner     (501) staff       (20)      576 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/Component.py
--rw-r--r--   0 runner     (501) staff       (20)      743 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/EditorExtension.py
--rw-r--r--   0 runner     (501) staff       (20)     3381 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/Font.py
--rw-r--r--   0 runner     (501) staff       (20)     1675 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/GameObject.py
--rw-r--r--   0 runner     (501) staff       (20)     2213 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/Material.py
--rw-r--r--   0 runner     (501) staff       (20)    42099 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/Mesh.py
--rw-r--r--   0 runner     (501) staff       (20)      194 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/MeshFilter.py
--rw-r--r--   0 runner     (501) staff       (20)      135 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/MeshRenderer.py
--rw-r--r--   0 runner     (501) staff       (20)     1515 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/MonoBehaviour.py
--rw-r--r--   0 runner     (501) staff       (20)      860 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/MonoScript.py
--rw-r--r--   0 runner     (501) staff       (20)      346 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/MovieTexture.py
--rw-r--r--   0 runner     (501) staff       (20)      500 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/NamedObject.py
--rw-r--r--   0 runner     (501) staff       (20)     6320 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/Object.py
--rw-r--r--   0 runner     (501) staff       (20)     3875 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/PPtr.py
--rw-r--r--   0 runner     (501) staff       (20)     1244 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/PlayerSettings.py
--rw-r--r--   0 runner     (501) staff       (20)      139 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/RectTransform.py
--rw-r--r--   0 runner     (501) staff       (20)     3848 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/Renderer.py
--rw-r--r--   0 runner     (501) staff       (20)      793 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/ResourceManager.py
--rw-r--r--   0 runner     (501) staff       (20)      157 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/RuntimeAnimatorController.py
--rw-r--r--   0 runner     (501) staff       (20)    17140 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/Shader.py
--rw-r--r--   0 runner     (501) staff       (20)      778 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/SkinnedMeshRenderer.py
--rw-r--r--   0 runner     (501) staff       (20)     9150 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/Sprite.py
--rw-r--r--   0 runner     (501) staff       (20)     1587 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/SpriteAtlas.py
--rw-r--r--   0 runner     (501) staff       (20)      939 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/TextAsset.py
--rw-r--r--   0 runner     (501) staff       (20)      926 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/Texture.py
--rw-r--r--   0 runner     (501) staff       (20)     9995 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/Texture2D.py
--rw-r--r--   0 runner     (501) staff       (20)      470 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/Transform.py
--rw-r--r--   0 runner     (501) staff       (20)     1829 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/VideoClip.py
--rw-r--r--   0 runner     (501) staff       (20)     1390 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/classes/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      379 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/config.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-03 16:40:40.127411 UnityPy-1.9.8/UnityPy/enums/
--rw-r--r--   0 runner     (501) staff       (20)     1189 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/enums/Audio.py
--rw-r--r--   0 runner     (501) staff       (20)      793 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/enums/BuildTarget.py
--rw-r--r--   0 runner     (501) staff       (20)    10278 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/enums/ClassIDType.py
--rw-r--r--   0 runner     (501) staff       (20)     2475 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/enums/CommonString.py
--rw-r--r--   0 runner     (501) staff       (20)      775 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/enums/ExtendableEnum.py
--rw-r--r--   0 runner     (501) staff       (20)      140 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/enums/FileType.py
--rw-r--r--   0 runner     (501) staff       (20)      220 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/enums/GfxPrimitiveType.py
--rw-r--r--   0 runner     (501) staff       (20)      119 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/enums/PassType.py
--rw-r--r--   0 runner     (501) staff       (20)      144 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/enums/SerializedPropertyType.py
--rw-r--r--   0 runner     (501) staff       (20)      815 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/enums/ShaderCompilerPlatform.py
--rw-r--r--   0 runner     (501) staff       (20)     1248 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/enums/ShaderGpuProgramType.py
--rw-r--r--   0 runner     (501) staff       (20)      119 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/enums/SpriteMeshType.py
--rw-r--r--   0 runner     (501) staff       (20)       99 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/enums/SpritePackingMode.py
--rw-r--r--   0 runner     (501) staff       (20)      176 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/enums/SpritePackingRotation.py
--rw-r--r--   0 runner     (501) staff       (20)      262 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/enums/TextureDimension.py
--rw-r--r--   0 runner     (501) staff       (20)     1265 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/enums/TextureFormat.py
--rw-r--r--   0 runner     (501) staff       (20)      707 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/enums/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     8716 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/environment.py
--rw-r--r--   0 runner     (501) staff       (20)      215 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/exceptions.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-03 16:40:40.130830 UnityPy-1.9.8/UnityPy/export/
--rw-r--r--   0 runner     (501) staff       (20)     9408 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/export/AudioClipConverter.py
--rw-r--r--   0 runner     (501) staff       (20)     2635 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/export/MeshExporter.py
--rw-r--r--   0 runner     (501) staff       (20)     5386 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/export/MeshRendererExporter.py
--rw-r--r--   0 runner     (501) staff       (20)    25167 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/export/ShaderConverter.py
--rw-r--r--   0 runner     (501) staff       (20)     5868 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/export/SpriteHelper.py
--rw-r--r--   0 runner     (501) staff       (20)    14360 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/export/Texture2DConverter.py
--rw-r--r--   0 runner     (501) staff       (20)      103 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/export/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-03 16:40:40.134075 UnityPy-1.9.8/UnityPy/files/
--rw-r--r--   0 runner     (501) staff       (20)    12899 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/files/BundleFile.py
--rw-r--r--   0 runner     (501) staff       (20)     5398 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/files/File.py
--rw-r--r--   0 runner     (501) staff       (20)     7824 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/files/ObjectReader.py
--rw-r--r--   0 runner     (501) staff       (20)    21434 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/files/SerializedFile.py
--rw-r--r--   0 runner     (501) staff       (20)     3693 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/files/WebFile.py
--rw-r--r--   0 runner     (501) staff       (20)      184 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/files/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-03 16:40:40.136813 UnityPy-1.9.8/UnityPy/helpers/
--rw-r--r--   0 runner     (501) staff       (20)     3511 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/helpers/CompressionHelper.py
--rw-r--r--   0 runner     (501) staff       (20)     3596 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/helpers/ImportHelper.py
--rw-r--r--   0 runner     (501) staff       (20)     2514 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/helpers/ResourceReader.py
--rw-r--r--   0 runner     (501) staff       (20)    14744 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/helpers/Tpk.py
--rw-r--r--   0 runner     (501) staff       (20)    16035 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/helpers/TypeTreeHelper.py
--rw-r--r--   0 runner     (501) staff       (20)       62 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/helpers/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-03 16:40:40.092224 UnityPy-1.9.8/UnityPy/lib/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-03 16:40:40.092350 UnityPy-1.9.8/UnityPy/lib/FMOD/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-03 16:40:40.092485 UnityPy-1.9.8/UnityPy/lib/FMOD/Darwin/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-03 16:40:40.137261 UnityPy-1.9.8/UnityPy/lib/FMOD/Darwin/x64/
--rw-r--r--   0 runner     (501) staff       (20)  2693392 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/lib/FMOD/Darwin/x64/libfmod.dylib
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-03 16:40:40.147435 UnityPy-1.9.8/UnityPy/math/
--rw-r--r--   0 runner     (501) staff       (20)     1539 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/math/Color.py
--rw-r--r--   0 runner     (501) staff       (20)     2782 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/math/Half.py
--rw-r--r--   0 runner     (501) staff       (20)     5523 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/math/Matrix4x4.py
--rw-r--r--   0 runner     (501) staff       (20)     1038 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/math/Quaternion.py
--rw-r--r--   0 runner     (501) staff       (20)      860 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/math/Rectangle.py
--rw-r--r--   0 runner     (501) staff       (20)     3816 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/math/Vector2.py
--rw-r--r--   0 runner     (501) staff       (20)     2403 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/math/Vector3.py
--rw-r--r--   0 runner     (501) staff       (20)     4154 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/math/Vector4.py
--rw-r--r--   0 runner     (501) staff       (20)      213 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/math/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-03 16:40:40.148781 UnityPy-1.9.8/UnityPy/resources/
--rw-r--r--   0 runner     (501) staff       (20)  1029887 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/resources/uncompressed.tpk
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-03 16:40:40.152559 UnityPy-1.9.8/UnityPy/streams/
--rw-r--r--   0 runner     (501) staff       (20)    16967 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/streams/EndianBinaryReader.py
--rw-r--r--   0 runner     (501) staff       (20)     5263 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/streams/EndianBinaryWriter.py
--rw-r--r--   0 runner     (501) staff       (20)      102 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPy/streams/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-03 16:40:40.099670 UnityPy-1.9.8/UnityPy.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)    12682 2022-08-03 16:40:40.000000 UnityPy-1.9.8/UnityPy.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3109 2022-08-03 16:40:40.000000 UnityPy-1.9.8/UnityPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-08-03 16:40:40.000000 UnityPy-1.9.8/UnityPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       51 2022-08-03 16:40:40.000000 UnityPy-1.9.8/UnityPy.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        8 2022-08-03 16:40:40.000000 UnityPy-1.9.8/UnityPy.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-03 16:40:40.154842 UnityPy-1.9.8/UnityPyBoost/
--rw-r--r--   0 runner     (501) staff       (20)     4210 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPyBoost/AnimationClip.c
--rw-r--r--   0 runner     (501) staff       (20)     6533 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPyBoost/Mesh.c
--rw-r--r--   0 runner     (501) staff       (20)    23746 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPyBoost/TypeTreeHelper.c
--rw-r--r--   0 runner     (501) staff       (20)     1417 2022-08-03 16:39:04.000000 UnityPy-1.9.8/UnityPyBoost/UnityPyBoost.c
--rw-r--r--   0 runner     (501) staff       (20)       79 2022-08-03 16:40:40.156170 UnityPy-1.9.8/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     3655 2022-08-03 16:39:05.000000 UnityPy-1.9.8/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 09:36:45.460083 UnityPy-1.9.9/
+-rw-r--r--   0 runner     (501) staff       (20)     1067 2022-08-04 09:34:11.000000 UnityPy-1.9.9/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)    12682 2022-08-04 09:36:45.460307 UnityPy-1.9.9/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    11652 2022-08-04 09:34:11.000000 UnityPy-1.9.9/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 09:36:43.661760 UnityPy-1.9.9/UnityPy/
+-rw-r--r--   0 runner     (501) staff       (20)      164 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 09:36:44.938617 UnityPy-1.9.9/UnityPy/classes/
+-rw-r--r--   0 runner     (501) staff       (20)      315 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/Animation.py
+-rw-r--r--   0 runner     (501) staff       (20)    20197 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/AnimationClip.py
+-rw-r--r--   0 runner     (501) staff       (20)     1352 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/Animator.py
+-rw-r--r--   0 runner     (501) staff       (20)    10915 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/AnimatorController.py
+-rw-r--r--   0 runner     (501) staff       (20)      553 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/AnimatorOverrideController.py
+-rw-r--r--   0 runner     (501) staff       (20)      769 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/AssetBundle.py
+-rw-r--r--   0 runner     (501) staff       (20)     2520 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/AudioClip.py
+-rw-r--r--   0 runner     (501) staff       (20)     5045 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/Avatar.py
+-rw-r--r--   0 runner     (501) staff       (20)      575 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/Behaviour.py
+-rw-r--r--   0 runner     (501) staff       (20)      448 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/BuildSettings.py
+-rw-r--r--   0 runner     (501) staff       (20)      576 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/Component.py
+-rw-r--r--   0 runner     (501) staff       (20)      743 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/EditorExtension.py
+-rw-r--r--   0 runner     (501) staff       (20)     3381 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/Font.py
+-rw-r--r--   0 runner     (501) staff       (20)     1675 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/GameObject.py
+-rw-r--r--   0 runner     (501) staff       (20)     2213 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/Material.py
+-rw-r--r--   0 runner     (501) staff       (20)    42099 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/Mesh.py
+-rw-r--r--   0 runner     (501) staff       (20)      194 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/MeshFilter.py
+-rw-r--r--   0 runner     (501) staff       (20)      135 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/MeshRenderer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1515 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/MonoBehaviour.py
+-rw-r--r--   0 runner     (501) staff       (20)      860 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/MonoScript.py
+-rw-r--r--   0 runner     (501) staff       (20)      346 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/MovieTexture.py
+-rw-r--r--   0 runner     (501) staff       (20)      500 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/NamedObject.py
+-rw-r--r--   0 runner     (501) staff       (20)     6320 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/Object.py
+-rw-r--r--   0 runner     (501) staff       (20)     3875 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/PPtr.py
+-rw-r--r--   0 runner     (501) staff       (20)     1244 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/PlayerSettings.py
+-rw-r--r--   0 runner     (501) staff       (20)      139 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/RectTransform.py
+-rw-r--r--   0 runner     (501) staff       (20)     3848 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/Renderer.py
+-rw-r--r--   0 runner     (501) staff       (20)      793 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/ResourceManager.py
+-rw-r--r--   0 runner     (501) staff       (20)      157 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/RuntimeAnimatorController.py
+-rw-r--r--   0 runner     (501) staff       (20)    17140 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/Shader.py
+-rw-r--r--   0 runner     (501) staff       (20)      778 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/SkinnedMeshRenderer.py
+-rw-r--r--   0 runner     (501) staff       (20)     9150 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/Sprite.py
+-rw-r--r--   0 runner     (501) staff       (20)     1587 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/SpriteAtlas.py
+-rw-r--r--   0 runner     (501) staff       (20)      939 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/TextAsset.py
+-rw-r--r--   0 runner     (501) staff       (20)      926 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/Texture.py
+-rw-r--r--   0 runner     (501) staff       (20)     9995 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/Texture2D.py
+-rw-r--r--   0 runner     (501) staff       (20)      470 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/Transform.py
+-rw-r--r--   0 runner     (501) staff       (20)     1829 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/VideoClip.py
+-rw-r--r--   0 runner     (501) staff       (20)     1390 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/classes/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      379 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/config.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 09:36:44.985346 UnityPy-1.9.9/UnityPy/enums/
+-rw-r--r--   0 runner     (501) staff       (20)     1189 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/enums/Audio.py
+-rw-r--r--   0 runner     (501) staff       (20)      793 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/enums/BuildTarget.py
+-rw-r--r--   0 runner     (501) staff       (20)    10278 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/enums/ClassIDType.py
+-rw-r--r--   0 runner     (501) staff       (20)     2475 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/enums/CommonString.py
+-rw-r--r--   0 runner     (501) staff       (20)      775 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/enums/ExtendableEnum.py
+-rw-r--r--   0 runner     (501) staff       (20)      140 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/enums/FileType.py
+-rw-r--r--   0 runner     (501) staff       (20)      220 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/enums/GfxPrimitiveType.py
+-rw-r--r--   0 runner     (501) staff       (20)      119 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/enums/PassType.py
+-rw-r--r--   0 runner     (501) staff       (20)      144 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/enums/SerializedPropertyType.py
+-rw-r--r--   0 runner     (501) staff       (20)      815 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/enums/ShaderCompilerPlatform.py
+-rw-r--r--   0 runner     (501) staff       (20)     1248 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/enums/ShaderGpuProgramType.py
+-rw-r--r--   0 runner     (501) staff       (20)      119 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/enums/SpriteMeshType.py
+-rw-r--r--   0 runner     (501) staff       (20)       99 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/enums/SpritePackingMode.py
+-rw-r--r--   0 runner     (501) staff       (20)      176 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/enums/SpritePackingRotation.py
+-rw-r--r--   0 runner     (501) staff       (20)      262 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/enums/TextureDimension.py
+-rw-r--r--   0 runner     (501) staff       (20)     1265 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/enums/TextureFormat.py
+-rw-r--r--   0 runner     (501) staff       (20)      707 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/enums/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     8716 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/environment.py
+-rw-r--r--   0 runner     (501) staff       (20)      215 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/exceptions.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 09:36:44.989007 UnityPy-1.9.9/UnityPy/export/
+-rw-r--r--   0 runner     (501) staff       (20)     9408 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/export/AudioClipConverter.py
+-rw-r--r--   0 runner     (501) staff       (20)     2635 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/export/MeshExporter.py
+-rw-r--r--   0 runner     (501) staff       (20)     5386 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/export/MeshRendererExporter.py
+-rw-r--r--   0 runner     (501) staff       (20)    25167 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/export/ShaderConverter.py
+-rw-r--r--   0 runner     (501) staff       (20)     5868 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/export/SpriteHelper.py
+-rw-r--r--   0 runner     (501) staff       (20)    14360 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/export/Texture2DConverter.py
+-rw-r--r--   0 runner     (501) staff       (20)      103 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/export/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 09:36:44.992279 UnityPy-1.9.9/UnityPy/files/
+-rw-r--r--   0 runner     (501) staff       (20)    12899 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/files/BundleFile.py
+-rw-r--r--   0 runner     (501) staff       (20)     5398 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/files/File.py
+-rw-r--r--   0 runner     (501) staff       (20)     7824 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/files/ObjectReader.py
+-rw-r--r--   0 runner     (501) staff       (20)    21434 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/files/SerializedFile.py
+-rw-r--r--   0 runner     (501) staff       (20)     3693 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/files/WebFile.py
+-rw-r--r--   0 runner     (501) staff       (20)      184 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/files/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 09:36:45.159817 UnityPy-1.9.9/UnityPy/helpers/
+-rw-r--r--   0 runner     (501) staff       (20)     3511 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/helpers/CompressionHelper.py
+-rw-r--r--   0 runner     (501) staff       (20)     3596 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/helpers/ImportHelper.py
+-rw-r--r--   0 runner     (501) staff       (20)     2514 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/helpers/ResourceReader.py
+-rw-r--r--   0 runner     (501) staff       (20)    14744 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/helpers/Tpk.py
+-rw-r--r--   0 runner     (501) staff       (20)    16037 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/helpers/TypeTreeHelper.py
+-rw-r--r--   0 runner     (501) staff       (20)       62 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/helpers/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 09:36:43.249919 UnityPy-1.9.9/UnityPy/lib/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 09:36:43.250046 UnityPy-1.9.9/UnityPy/lib/FMOD/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 09:36:43.250174 UnityPy-1.9.9/UnityPy/lib/FMOD/Darwin/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 09:36:45.242446 UnityPy-1.9.9/UnityPy/lib/FMOD/Darwin/x64/
+-rw-r--r--   0 runner     (501) staff       (20)  2693392 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/lib/FMOD/Darwin/x64/libfmod.dylib
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 09:36:45.291625 UnityPy-1.9.9/UnityPy/math/
+-rw-r--r--   0 runner     (501) staff       (20)     1539 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/math/Color.py
+-rw-r--r--   0 runner     (501) staff       (20)     2782 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/math/Half.py
+-rw-r--r--   0 runner     (501) staff       (20)     5523 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/math/Matrix4x4.py
+-rw-r--r--   0 runner     (501) staff       (20)     1038 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/math/Quaternion.py
+-rw-r--r--   0 runner     (501) staff       (20)      860 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/math/Rectangle.py
+-rw-r--r--   0 runner     (501) staff       (20)     3816 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/math/Vector2.py
+-rw-r--r--   0 runner     (501) staff       (20)     2403 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/math/Vector3.py
+-rw-r--r--   0 runner     (501) staff       (20)     4154 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/math/Vector4.py
+-rw-r--r--   0 runner     (501) staff       (20)      213 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/math/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 09:36:45.292129 UnityPy-1.9.9/UnityPy/resources/
+-rw-r--r--   0 runner     (501) staff       (20)  1029887 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/resources/uncompressed.tpk
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 09:36:45.295580 UnityPy-1.9.9/UnityPy/streams/
+-rw-r--r--   0 runner     (501) staff       (20)    16967 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/streams/EndianBinaryReader.py
+-rw-r--r--   0 runner     (501) staff       (20)     5263 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/streams/EndianBinaryWriter.py
+-rw-r--r--   0 runner     (501) staff       (20)      102 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPy/streams/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 09:36:43.988895 UnityPy-1.9.9/UnityPy.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    12682 2022-08-04 09:36:42.000000 UnityPy-1.9.9/UnityPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3109 2022-08-04 09:36:43.000000 UnityPy-1.9.9/UnityPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-08-04 09:36:43.000000 UnityPy-1.9.9/UnityPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       51 2022-08-04 09:36:43.000000 UnityPy-1.9.9/UnityPy.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        8 2022-08-04 09:36:43.000000 UnityPy-1.9.9/UnityPy.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 09:36:45.418586 UnityPy-1.9.9/UnityPyBoost/
+-rw-r--r--   0 runner     (501) staff       (20)     4210 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPyBoost/AnimationClip.c
+-rw-r--r--   0 runner     (501) staff       (20)     6533 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPyBoost/Mesh.c
+-rw-r--r--   0 runner     (501) staff       (20)    23746 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPyBoost/TypeTreeHelper.c
+-rw-r--r--   0 runner     (501) staff       (20)     1417 2022-08-04 09:34:11.000000 UnityPy-1.9.9/UnityPyBoost/UnityPyBoost.c
+-rw-r--r--   0 runner     (501) staff       (20)       79 2022-08-04 09:36:45.461192 UnityPy-1.9.9/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     3605 2022-08-04 09:34:11.000000 UnityPy-1.9.9/setup.py
```

### Comparing `UnityPy-1.9.8/LICENSE` & `UnityPy-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/PKG-INFO` & `UnityPy-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnityPy
-Version: 1.9.8
+Version: 1.9.9
 Summary: A pythonic port of AssetStudio by Perfare
 Home-page: https://github.com/K0lb3/UnityPy
 Download-URL: https://github.com/K0lb3/UnityPy/tarball/master
 Author: K0lb3
 Keywords: python,unity,unity-asset,python3,data-minig,unitypack,assetstudio,unity-asset-extractor
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `UnityPy-1.9.8/README.md` & `UnityPy-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/AnimationClip.py` & `UnityPy-1.9.9/UnityPy/classes/AnimationClip.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/Animator.py` & `UnityPy-1.9.9/UnityPy/classes/Animator.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/AnimatorController.py` & `UnityPy-1.9.9/UnityPy/classes/AnimatorController.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/AnimatorOverrideController.py` & `UnityPy-1.9.9/UnityPy/classes/AnimatorOverrideController.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/AssetBundle.py` & `UnityPy-1.9.9/UnityPy/classes/AssetBundle.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/AudioClip.py` & `UnityPy-1.9.9/UnityPy/classes/AudioClip.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/Avatar.py` & `UnityPy-1.9.9/UnityPy/classes/Avatar.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/Behaviour.py` & `UnityPy-1.9.9/UnityPy/classes/Behaviour.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/Component.py` & `UnityPy-1.9.9/UnityPy/classes/Component.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/EditorExtension.py` & `UnityPy-1.9.9/UnityPy/classes/EditorExtension.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/Font.py` & `UnityPy-1.9.9/UnityPy/classes/Font.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/GameObject.py` & `UnityPy-1.9.9/UnityPy/classes/GameObject.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/Material.py` & `UnityPy-1.9.9/UnityPy/classes/Material.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/Mesh.py` & `UnityPy-1.9.9/UnityPy/classes/Mesh.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/MonoBehaviour.py` & `UnityPy-1.9.9/UnityPy/classes/MonoBehaviour.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/MonoScript.py` & `UnityPy-1.9.9/UnityPy/classes/MonoScript.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/Object.py` & `UnityPy-1.9.9/UnityPy/classes/Object.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/PPtr.py` & `UnityPy-1.9.9/UnityPy/classes/PPtr.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/PlayerSettings.py` & `UnityPy-1.9.9/UnityPy/classes/PlayerSettings.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/Renderer.py` & `UnityPy-1.9.9/UnityPy/classes/Renderer.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/ResourceManager.py` & `UnityPy-1.9.9/UnityPy/classes/ResourceManager.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/Shader.py` & `UnityPy-1.9.9/UnityPy/classes/Shader.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/SkinnedMeshRenderer.py` & `UnityPy-1.9.9/UnityPy/classes/SkinnedMeshRenderer.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/Sprite.py` & `UnityPy-1.9.9/UnityPy/classes/Sprite.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/SpriteAtlas.py` & `UnityPy-1.9.9/UnityPy/classes/SpriteAtlas.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/TextAsset.py` & `UnityPy-1.9.9/UnityPy/classes/TextAsset.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/Texture.py` & `UnityPy-1.9.9/UnityPy/classes/Texture.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/Texture2D.py` & `UnityPy-1.9.9/UnityPy/classes/Texture2D.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/VideoClip.py` & `UnityPy-1.9.9/UnityPy/classes/VideoClip.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/classes/__init__.py` & `UnityPy-1.9.9/UnityPy/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/enums/Audio.py` & `UnityPy-1.9.9/UnityPy/enums/Audio.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/enums/BuildTarget.py` & `UnityPy-1.9.9/UnityPy/enums/BuildTarget.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/enums/ClassIDType.py` & `UnityPy-1.9.9/UnityPy/enums/ClassIDType.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/enums/CommonString.py` & `UnityPy-1.9.9/UnityPy/enums/CommonString.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/enums/ExtendableEnum.py` & `UnityPy-1.9.9/UnityPy/enums/ExtendableEnum.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/enums/ShaderCompilerPlatform.py` & `UnityPy-1.9.9/UnityPy/enums/ShaderCompilerPlatform.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/enums/ShaderGpuProgramType.py` & `UnityPy-1.9.9/UnityPy/enums/ShaderGpuProgramType.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/enums/TextureFormat.py` & `UnityPy-1.9.9/UnityPy/enums/TextureFormat.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/enums/__init__.py` & `UnityPy-1.9.9/UnityPy/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/environment.py` & `UnityPy-1.9.9/UnityPy/environment.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/export/AudioClipConverter.py` & `UnityPy-1.9.9/UnityPy/export/AudioClipConverter.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/export/MeshExporter.py` & `UnityPy-1.9.9/UnityPy/export/MeshExporter.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/export/MeshRendererExporter.py` & `UnityPy-1.9.9/UnityPy/export/MeshRendererExporter.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/export/ShaderConverter.py` & `UnityPy-1.9.9/UnityPy/export/ShaderConverter.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/export/SpriteHelper.py` & `UnityPy-1.9.9/UnityPy/export/SpriteHelper.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/export/Texture2DConverter.py` & `UnityPy-1.9.9/UnityPy/export/Texture2DConverter.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/files/BundleFile.py` & `UnityPy-1.9.9/UnityPy/files/BundleFile.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/files/File.py` & `UnityPy-1.9.9/UnityPy/files/File.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/files/ObjectReader.py` & `UnityPy-1.9.9/UnityPy/files/ObjectReader.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/files/SerializedFile.py` & `UnityPy-1.9.9/UnityPy/files/SerializedFile.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/files/WebFile.py` & `UnityPy-1.9.9/UnityPy/files/WebFile.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/helpers/CompressionHelper.py` & `UnityPy-1.9.9/UnityPy/helpers/CompressionHelper.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/helpers/ImportHelper.py` & `UnityPy-1.9.9/UnityPy/helpers/ImportHelper.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/helpers/ResourceReader.py` & `UnityPy-1.9.9/UnityPy/helpers/ResourceReader.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/helpers/Tpk.py` & `UnityPy-1.9.9/UnityPy/helpers/Tpk.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/helpers/TypeTreeHelper.py` & `UnityPy-1.9.9/UnityPy/helpers/TypeTreeHelper.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,13 +512,13 @@
             for val in value:
                 write_value(val, vector, writer, c_uint32(3))
         else:  # Class
             clz = get_nodes(nodes, i.value)
             i.value += len(clz) - 1
             j = c_uint32(1)
             while j.value < len(clz):
-                val = value[clz[j.value].name]
+                val = value[clz[j.value].m_Name]
                 write_value(val, clz, writer, j)
                 j.value += 1
 
     if align:
         writer.align_stream()
```

### Comparing `UnityPy-1.9.8/UnityPy/lib/FMOD/Darwin/x64/libfmod.dylib` & `UnityPy-1.9.9/UnityPy/lib/FMOD/Darwin/x64/libfmod.dylib`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/math/Color.py` & `UnityPy-1.9.9/UnityPy/math/Color.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/math/Half.py` & `UnityPy-1.9.9/UnityPy/math/Half.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/math/Matrix4x4.py` & `UnityPy-1.9.9/UnityPy/math/Matrix4x4.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/math/Quaternion.py` & `UnityPy-1.9.9/UnityPy/math/Quaternion.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/math/Rectangle.py` & `UnityPy-1.9.9/UnityPy/math/Rectangle.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/math/Vector2.py` & `UnityPy-1.9.9/UnityPy/math/Vector2.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/math/Vector3.py` & `UnityPy-1.9.9/UnityPy/math/Vector3.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/math/Vector4.py` & `UnityPy-1.9.9/UnityPy/math/Vector4.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/resources/uncompressed.tpk` & `UnityPy-1.9.9/UnityPy/resources/uncompressed.tpk`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/streams/EndianBinaryReader.py` & `UnityPy-1.9.9/UnityPy/streams/EndianBinaryReader.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy/streams/EndianBinaryWriter.py` & `UnityPy-1.9.9/UnityPy/streams/EndianBinaryWriter.py`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPy.egg-info/PKG-INFO` & `UnityPy-1.9.9/UnityPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnityPy
-Version: 1.9.8
+Version: 1.9.9
 Summary: A pythonic port of AssetStudio by Perfare
 Home-page: https://github.com/K0lb3/UnityPy
 Download-URL: https://github.com/K0lb3/UnityPy/tarball/master
 Author: K0lb3
 Keywords: python,unity,unity-asset,python3,data-minig,unitypack,assetstudio,unity-asset-extractor
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `UnityPy-1.9.8/UnityPy.egg-info/SOURCES.txt` & `UnityPy-1.9.9/UnityPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPyBoost/AnimationClip.c` & `UnityPy-1.9.9/UnityPyBoost/AnimationClip.c`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPyBoost/Mesh.c` & `UnityPy-1.9.9/UnityPyBoost/Mesh.c`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPyBoost/TypeTreeHelper.c` & `UnityPy-1.9.9/UnityPyBoost/TypeTreeHelper.c`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/UnityPyBoost/UnityPyBoost.c` & `UnityPy-1.9.9/UnityPyBoost/UnityPyBoost.c`

 * *Files identical despite different names*

### Comparing `UnityPy-1.9.8/setup.py` & `UnityPy-1.9.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,24 +48,21 @@
 
     return f"lib/FMOD/{system}/{arch}/{lib_name}"
 
 
 setup(
     name="UnityPy",
     packages=find_packages(),
-    #include_package_data=True,
+    # include_package_data=True,
     package_data={
         "UnityPy": [
             get_fmod_library(),
             "resources/uncompressed.tpk",
-            "*.c",
-            "*.h",
-            "*.cpp",
-            "*.hpp",
-        ]
+        ],
+        "": ["*.c", "*.h"],
     },
     version=version,
     author="K0lb3",
     description="A pythonic port of AssetStudio by Perfare",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/K0lb3/UnityPy",
```

