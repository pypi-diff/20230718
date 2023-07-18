# Comparing `tmp/systembridgewindowssensors-3.8.0.dev8.tar.gz` & `tmp/systembridgewindowssensors-3.8.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgewindowssensors-3.8.0.dev8.tar", last modified: Tue Jul 18 10:21:44 2023, max compression
+gzip compressed data, was "systembridgewindowssensors-3.8.0.dev9.tar", last modified: Tue Jul 18 14:40:16 2023, max compression
```

## Comparing `systembridgewindowssensors-3.8.0.dev8.tar` & `systembridgewindowssensors-3.8.0.dev9.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.487654 systembridgewindowssensors-3.8.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-18 10:21:44.487654 systembridgewindowssensors-3.8.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-18 10:21:04.000000 systembridgewindowssensors-3.8.0.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 10:21:44.487654 systembridgewindowssensors-3.8.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-18 10:21:04.000000 systembridgewindowssensors-3.8.0.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.475653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-18 10:21:04.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-18 10:21:42.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.475653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.475653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/lib/netstandard2.0/
--rw-r--r--   0 runner    (1001) docker     (123)   189504 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/lib/netstandard2.0/Mono.Posix.NETStandard.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.475653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/native/
--rw-r--r--   0 runner    (1001) docker     (123)   183240 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/native/libMonoPosixHelper.so
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/native/libSystem.IO.Ports.Native.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.475653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/lib/netstandard2.0/
--rw-r--r--   0 runner    (1001) docker     (123)   189504 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/lib/netstandard2.0/Mono.Posix.NETStandard.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.475653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/native/
--rw-r--r--   0 runner    (1001) docker     (123)   246736 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/native/libMonoPosixHelper.so
--rw-r--r--   0 runner    (1001) docker     (123)   200200 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/native/libSystem.IO.Ports.Native.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-armel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-armel/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.475653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-armel/lib/netstandard2.0/
--rw-r--r--   0 runner    (1001) docker     (123)   189504 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-armel/lib/netstandard2.0/Mono.Posix.NETStandard.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.475653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-armel/native/
--rw-r--r--   0 runner    (1001) docker     (123)   236480 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-armel/native/libMonoPosixHelper.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.479653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/lib/netstandard2.0/
--rw-r--r--   0 runner    (1001) docker     (123)   189504 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/lib/netstandard2.0/Mono.Posix.NETStandard.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.479653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/native/
--rw-r--r--   0 runner    (1001) docker     (123)   920882 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/native/libMonoPosixHelper.so
--rw-r--r--   0 runner    (1001) docker     (123)    24120 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/native/libSystem.IO.Ports.Native.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x86/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x86/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.479653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x86/lib/netstandard2.0/
--rw-r--r--   0 runner    (1001) docker     (123)   189504 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x86/lib/netstandard2.0/Mono.Posix.NETStandard.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.479653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x86/native/
--rw-r--r--   0 runner    (1001) docker     (123)   766620 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x86/native/libMonoPosixHelper.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.479653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx/lib/netstandard2.0/
--rw-r--r--   0 runner    (1001) docker     (123)   189504 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx/lib/netstandard2.0/Mono.Posix.NETStandard.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.479653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx/native/
--rw-r--r--   0 runner    (1001) docker     (123)   535888 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx/native/libMonoPosixHelper.dylib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx-arm64/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.479653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx-arm64/native/
--rw-r--r--   0 runner    (1001) docker     (123)    70464 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx-arm64/native/libSystem.IO.Ports.Native.dylib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx-x64/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.479653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx-x64/native/
--rw-r--r--   0 runner    (1001) docker     (123)    53968 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx-x64/native/libSystem.IO.Ports.Native.dylib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/unix/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/unix/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.483653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/unix/lib/net7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    75904 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/unix/lib/net7.0/System.IO.Ports.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.475653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.475653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.487654 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win/lib/net7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    87168 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win/lib/net7.0/System.IO.Ports.dll
--rw-r--r--   0 runner    (1001) docker     (123)   295600 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win/lib/net7.0/System.Management.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.471653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.483653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/lib/netstandard2.0/
--rw-r--r--   0 runner    (1001) docker     (123)   189504 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/lib/netstandard2.0/Mono.Posix.NETStandard.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.483653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/native/
--rw-r--r--   0 runner    (1001) docker     (123)    87600 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/native/MonoPosixHelper.dll
--rw-r--r--   0 runner    (1001) docker     (123)  1495800 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/native/libMonoPosixHelper.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.475653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.475653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.483653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/lib/netstandard2.0/
--rw-r--r--   0 runner    (1001) docker     (123)   189504 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/lib/netstandard2.0/Mono.Posix.NETStandard.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.483653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/native/
--rw-r--r--   0 runner    (1001) docker     (123)   400120 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/native/MonoPosixHelper.dll
--rw-r--r--   0 runner    (1001) docker     (123)  1256296 2023-07-18 10:21:05.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/native/libMonoPosixHelper.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:21:44.475653 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-18 10:21:44.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-18 10:21:44.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:21:44.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 10:21:44.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-18 10:21:44.000000 systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.857397 systembridgewindowssensors-3.8.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-18 14:40:16.857397 systembridgewindowssensors-3.8.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-18 14:39:35.000000 systembridgewindowssensors-3.8.0.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:40:16.857397 systembridgewindowssensors-3.8.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-18 14:39:35.000000 systembridgewindowssensors-3.8.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-18 14:39:35.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-18 14:40:14.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.837397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.837397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/lib/netstandard2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   189504 2023-07-18 14:39:36.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/lib/netstandard2.0/Mono.Posix.NETStandard.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.845397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/native/
+-rw-r--r--   0 runner    (1001) docker     (123)   183240 2023-07-18 14:39:36.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/native/libMonoPosixHelper.so
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-07-18 14:39:36.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/native/libSystem.IO.Ports.Native.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.845397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/lib/netstandard2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   189504 2023-07-18 14:39:36.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/lib/netstandard2.0/Mono.Posix.NETStandard.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.845397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/native/
+-rw-r--r--   0 runner    (1001) docker     (123)   246736 2023-07-18 14:39:36.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/native/libMonoPosixHelper.so
+-rw-r--r--   0 runner    (1001) docker     (123)   200200 2023-07-18 14:39:36.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/native/libSystem.IO.Ports.Native.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-armel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-armel/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.845397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-armel/lib/netstandard2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   189504 2023-07-18 14:39:36.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-armel/lib/netstandard2.0/Mono.Posix.NETStandard.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.845397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-armel/native/
+-rw-r--r--   0 runner    (1001) docker     (123)   236480 2023-07-18 14:39:36.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-armel/native/libMonoPosixHelper.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.845397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/lib/netstandard2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   189504 2023-07-18 14:39:36.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/lib/netstandard2.0/Mono.Posix.NETStandard.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.845397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/native/
+-rw-r--r--   0 runner    (1001) docker     (123)   920882 2023-07-18 14:39:36.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/native/libMonoPosixHelper.so
+-rw-r--r--   0 runner    (1001) docker     (123)    24120 2023-07-18 14:39:36.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/native/libSystem.IO.Ports.Native.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x86/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x86/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.845397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x86/lib/netstandard2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   189504 2023-07-18 14:39:36.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x86/lib/netstandard2.0/Mono.Posix.NETStandard.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.849397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x86/native/
+-rw-r--r--   0 runner    (1001) docker     (123)   766620 2023-07-18 14:39:37.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x86/native/libMonoPosixHelper.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.849397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx/lib/netstandard2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   189504 2023-07-18 14:39:37.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx/lib/netstandard2.0/Mono.Posix.NETStandard.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.849397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx/native/
+-rw-r--r--   0 runner    (1001) docker     (123)   535888 2023-07-18 14:39:37.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx/native/libMonoPosixHelper.dylib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx-arm64/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.849397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx-arm64/native/
+-rw-r--r--   0 runner    (1001) docker     (123)    70464 2023-07-18 14:39:37.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx-arm64/native/libSystem.IO.Ports.Native.dylib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx-x64/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.849397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx-x64/native/
+-rw-r--r--   0 runner    (1001) docker     (123)    53968 2023-07-18 14:39:37.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx-x64/native/libSystem.IO.Ports.Native.dylib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/unix/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/unix/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.849397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/unix/lib/net7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    75904 2023-07-18 14:39:37.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/unix/lib/net7.0/System.IO.Ports.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.853397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win/lib/net7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    87168 2023-07-18 14:39:37.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win/lib/net7.0/System.IO.Ports.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   295600 2023-07-18 14:39:37.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win/lib/net7.0/System.Management.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.849397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/lib/netstandard2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   189504 2023-07-18 14:39:37.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/lib/netstandard2.0/Mono.Posix.NETStandard.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.849397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/native/
+-rw-r--r--   0 runner    (1001) docker     (123)    87600 2023-07-18 14:39:37.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/native/MonoPosixHelper.dll
+-rw-r--r--   0 runner    (1001) docker     (123)  1495800 2023-07-18 14:39:37.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/native/libMonoPosixHelper.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.853397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/lib/netstandard2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   189504 2023-07-18 14:39:37.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/lib/netstandard2.0/Mono.Posix.NETStandard.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.853397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/native/
+-rw-r--r--   0 runner    (1001) docker     (123)   400120 2023-07-18 14:39:37.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/native/MonoPosixHelper.dll
+-rw-r--r--   0 runner    (1001) docker     (123)  1256296 2023-07-18 14:39:37.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/native/libMonoPosixHelper.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:40:16.841397 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-18 14:40:16.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-18 14:40:16.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:40:16.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 14:40:16.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-18 14:40:16.000000 systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors.egg-info/top_level.txt
```

### Comparing `systembridgewindowssensors-3.8.0.dev8/pyproject.toml` & `systembridgewindowssensors-3.8.0.dev9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/setup.py` & `systembridgewindowssensors-3.8.0.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/lib/netstandard2.0/Mono.Posix.NETStandard.dll` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/lib/netstandard2.0/Mono.Posix.NETStandard.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/native/libMonoPosixHelper.so` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/native/libMonoPosixHelper.so`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/native/libSystem.IO.Ports.Native.so` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm/native/libSystem.IO.Ports.Native.so`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/lib/netstandard2.0/Mono.Posix.NETStandard.dll` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/lib/netstandard2.0/Mono.Posix.NETStandard.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/native/libMonoPosixHelper.so` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/native/libMonoPosixHelper.so`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/native/libSystem.IO.Ports.Native.so` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-arm64/native/libSystem.IO.Ports.Native.so`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-armel/lib/netstandard2.0/Mono.Posix.NETStandard.dll` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-armel/lib/netstandard2.0/Mono.Posix.NETStandard.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-armel/native/libMonoPosixHelper.so` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-armel/native/libMonoPosixHelper.so`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/lib/netstandard2.0/Mono.Posix.NETStandard.dll` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/lib/netstandard2.0/Mono.Posix.NETStandard.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/native/libMonoPosixHelper.so` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/native/libMonoPosixHelper.so`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/native/libSystem.IO.Ports.Native.so` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x64/native/libSystem.IO.Ports.Native.so`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x86/lib/netstandard2.0/Mono.Posix.NETStandard.dll` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x86/lib/netstandard2.0/Mono.Posix.NETStandard.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x86/native/libMonoPosixHelper.so` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/linux-x86/native/libMonoPosixHelper.so`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx/lib/netstandard2.0/Mono.Posix.NETStandard.dll` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx/lib/netstandard2.0/Mono.Posix.NETStandard.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx/native/libMonoPosixHelper.dylib` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx/native/libMonoPosixHelper.dylib`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx-arm64/native/libSystem.IO.Ports.Native.dylib` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx-arm64/native/libSystem.IO.Ports.Native.dylib`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx-x64/native/libSystem.IO.Ports.Native.dylib` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/osx-x64/native/libSystem.IO.Ports.Native.dylib`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/unix/lib/net7.0/System.IO.Ports.dll` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/unix/lib/net7.0/System.IO.Ports.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win/lib/net7.0/System.IO.Ports.dll` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win/lib/net7.0/System.IO.Ports.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win/lib/net7.0/System.Management.dll` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win/lib/net7.0/System.Management.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/lib/netstandard2.0/Mono.Posix.NETStandard.dll` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/lib/netstandard2.0/Mono.Posix.NETStandard.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/native/MonoPosixHelper.dll` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/native/MonoPosixHelper.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/native/libMonoPosixHelper.dll` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x64/native/libMonoPosixHelper.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/lib/netstandard2.0/Mono.Posix.NETStandard.dll` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/lib/netstandard2.0/Mono.Posix.NETStandard.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/native/MonoPosixHelper.dll` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/native/MonoPosixHelper.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/native/libMonoPosixHelper.dll` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors/bin/net7.0-windows/runtimes/win-x86/native/libMonoPosixHelper.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.8.0.dev8/systembridgewindowssensors.egg-info/SOURCES.txt` & `systembridgewindowssensors-3.8.0.dev9/systembridgewindowssensors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

