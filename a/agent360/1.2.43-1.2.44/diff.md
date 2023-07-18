# Comparing `tmp/agent360-1.2.43.tar.gz` & `tmp/agent360-1.2.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent360-1.2.43.tar", last modified: Thu May 11 21:18:50 2023, max compression
+gzip compressed data, was "agent360-1.2.44.tar", last modified: Tue May 16 14:08:29 2023, max compression
```

## Comparing `agent360-1.2.43.tar` & `agent360-1.2.44.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:18:50.249227 agent360-1.2.43/
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-11 21:18:41.000000 agent360-1.2.43/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 21:18:41.000000 agent360-1.2.43/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-11 21:18:50.249227 agent360-1.2.43/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-11 21:18:41.000000 agent360-1.2.43/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:18:50.241227 agent360-1.2.43/agent360/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25377 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/agent360.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:18:50.249227 agent360-1.2.43/agent360/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/apt-updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/asterisk.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/bind.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/bird.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/bitninja.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/cloudlinux-dbgov.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/cloudlinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/cpanel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2020 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/cpu_freq.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/dirsize.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/diskinodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/diskstatus-nvme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/diskstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4140 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/diskusage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/dovecot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/exim.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/fail2ban.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/haproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/httpd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5227 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/iostat.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/janus.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/kamailio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/litespeed.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      332 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/loadavg.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/loggedin.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/mailq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/mdstat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/megacli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/memcached.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      919 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/minecraft.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/openvpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/phpfpm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3165 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/ping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6330 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/plesk-cgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/postfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/powerdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/proftpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/redis_stat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      244 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/sleeper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/swap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/temp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/unbound.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/vms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/wp-toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360/plugins/yum-updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-11 21:18:41.000000 agent360-1.2.43/agent360-example.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:18:50.241227 agent360-1.2.43/agent360.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-11 21:18:50.000000 agent360-1.2.43/agent360.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-11 21:18:50.000000 agent360-1.2.43/agent360.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:18:50.000000 agent360-1.2.43/agent360.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 21:18:50.000000 agent360-1.2.43/agent360.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 21:18:50.000000 agent360-1.2.43/agent360.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 21:18:50.000000 agent360-1.2.43/agent360.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 21:18:50.249227 agent360-1.2.43/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-11 21:18:41.000000 agent360-1.2.43/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:08:29.398237 agent360-1.2.44/
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-16 14:08:20.000000 agent360-1.2.44/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 14:08:20.000000 agent360-1.2.44/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-16 14:08:29.398237 agent360-1.2.44/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-16 14:08:20.000000 agent360-1.2.44/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:08:29.382237 agent360-1.2.44/agent360/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25377 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/agent360.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:08:29.398237 agent360-1.2.44/agent360/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/apt-updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/asterisk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/bind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/bird.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/bitninja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/cloudlinux-dbgov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/cloudlinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/cpanel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2020 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/cpu_freq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/dirsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/diskinodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/diskstatus-nvme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/diskstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4140 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/diskusage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/dovecot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/exim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/fail2ban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/haproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/httpd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5227 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/iostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/janus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/kamailio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/litespeed.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      332 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/loadavg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/loggedin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/mailq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/mdstat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/megacli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/memcached.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      919 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/minecraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/openvpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/phpfpm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3165 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/ping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6330 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/plesk-cgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/postfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/powerdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/proftpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/redis_stat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      244 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/sleeper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/temp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/unbound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/vms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/wp-toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360/plugins/yum-updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-16 14:08:20.000000 agent360-1.2.44/agent360-example.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:08:29.386237 agent360-1.2.44/agent360.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-16 14:08:29.000000 agent360-1.2.44/agent360.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-16 14:08:29.000000 agent360-1.2.44/agent360.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:08:29.000000 agent360-1.2.44/agent360.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 14:08:29.000000 agent360-1.2.44/agent360.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 14:08:29.000000 agent360-1.2.44/agent360.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 14:08:29.000000 agent360-1.2.44/agent360.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 14:08:29.398237 agent360-1.2.44/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-16 14:08:20.000000 agent360-1.2.44/setup.py
```

### Comparing `agent360-1.2.43/LICENSE` & `agent360-1.2.44/LICENSE`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/PKG-INFO` & `agent360-1.2.44/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent360
-Version: 1.2.43
+Version: 1.2.44
 Summary: 360 agent
 Home-page: https://github.com/plesk/agent360
 Author: 360
 Author-email: 360support@webpros.com
 Maintainer: 360
 Maintainer-email: 360support@webpros.com
 License: BSD-3-Clause
```

### Comparing `agent360-1.2.43/README.md` & `agent360-1.2.44/README.md`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/agent360.py` & `agent360-1.2.44/agent360/agent360.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     from urllib.request import urlopen, Request
     from urllib.error import HTTPError
 except ImportError:
     from urlparse import urlparse
     from urllib import urlencode
     from urllib2 import urlopen, Request, HTTPError
 
-__version__ = '1.2.43'
+__version__ = '1.2.44'
 __FILEABSDIRNAME__ = os.path.dirname(os.path.abspath(__file__))
 
 ini_files = (
     os.path.join('/etc', 'agent360.ini'),
     os.path.join('/etc', 'agent360-custom.ini'),
     os.path.join('/etc', 'agent360-token.ini'),
     os.path.join(os.path.dirname(__FILEABSDIRNAME__), 'agent360.ini'),
```

### Comparing `agent360-1.2.43/agent360/plugins/apt-updates.py` & `agent360-1.2.44/agent360/plugins/apt-updates.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/asterisk.py` & `agent360-1.2.44/agent360/plugins/asterisk.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/bind.py` & `agent360-1.2.44/agent360/plugins/bind.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/bird.py` & `agent360-1.2.44/agent360/plugins/bird.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/bitninja.py` & `agent360-1.2.44/agent360/plugins/bitninja.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/cloudlinux-dbgov.py` & `agent360-1.2.44/agent360/plugins/cloudlinux-dbgov.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/cloudlinux.py` & `agent360-1.2.44/agent360/plugins/cloudlinux.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/cpanel.py` & `agent360-1.2.44/agent360/plugins/cpanel.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/cpu.py` & `agent360-1.2.44/agent360/plugins/cpu.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/cpu_freq.py` & `agent360-1.2.44/agent360/plugins/cpu_freq.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/dirsize.py` & `agent360-1.2.44/agent360/plugins/dirsize.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/diskinodes.py` & `agent360-1.2.44/agent360/plugins/diskinodes.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/diskstatus-nvme.py` & `agent360-1.2.44/agent360/plugins/diskstatus-nvme.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/diskstatus.py` & `agent360-1.2.44/agent360/plugins/diskstatus.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/diskusage.py` & `agent360-1.2.44/agent360/plugins/diskusage.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/docker.py` & `agent360-1.2.44/agent360/plugins/docker.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/dovecot.py` & `agent360-1.2.44/agent360/plugins/dovecot.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/elasticsearch.py` & `agent360-1.2.44/agent360/plugins/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/fail2ban.py` & `agent360-1.2.44/agent360/plugins/fail2ban.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/gpu.py` & `agent360-1.2.44/agent360/plugins/gpu.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/haproxy.py` & `agent360-1.2.44/agent360/plugins/haproxy.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/httpd.py` & `agent360-1.2.44/agent360/plugins/httpd.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/iostat.py` & `agent360-1.2.44/agent360/plugins/iostat.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/janus.py` & `agent360-1.2.44/agent360/plugins/janus.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/kamailio.py` & `agent360-1.2.44/agent360/plugins/kamailio.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/litespeed.py` & `agent360-1.2.44/agent360/plugins/litespeed.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/mailq.py` & `agent360-1.2.44/agent360/plugins/mailq.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/mdstat.py` & `agent360-1.2.44/agent360/plugins/mdstat.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/megacli.py` & `agent360-1.2.44/agent360/plugins/megacli.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/memcached.py` & `agent360-1.2.44/agent360/plugins/memcached.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/memory.py` & `agent360-1.2.44/agent360/plugins/memory.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/minecraft.py` & `agent360-1.2.44/agent360/plugins/minecraft.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/mongodb.py` & `agent360-1.2.44/agent360/plugins/mongodb.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/mysql.py` & `agent360-1.2.44/agent360/plugins/mysql.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/network.py` & `agent360-1.2.44/agent360/plugins/network.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/nginx.py` & `agent360-1.2.44/agent360/plugins/nginx.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/openvpn.py` & `agent360-1.2.44/agent360/plugins/openvpn.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/phpfpm.py` & `agent360-1.2.44/agent360/plugins/phpfpm.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/ping.py` & `agent360-1.2.44/agent360/plugins/ping.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/plesk-cgroups.py` & `agent360-1.2.44/agent360/plugins/plesk-cgroups.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/plugins.py` & `agent360-1.2.44/agent360/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/postfix.py` & `agent360-1.2.44/agent360/plugins/postfix.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/powerdns.py` & `agent360-1.2.44/agent360/plugins/powerdns.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/process.py` & `agent360-1.2.44/agent360/plugins/process.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/proftpd.py` & `agent360-1.2.44/agent360/plugins/proftpd.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/rabbitmq.py` & `agent360-1.2.44/agent360/plugins/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/redis_stat.py` & `agent360-1.2.44/agent360/plugins/redis_stat.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/system.py` & `agent360-1.2.44/agent360/plugins/system.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/temp.py` & `agent360-1.2.44/agent360/plugins/temp.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/unbound.py` & `agent360-1.2.44/agent360/plugins/unbound.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/vms.py` & `agent360-1.2.44/agent360/plugins/vms.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/wp-toolkit.py` & `agent360-1.2.44/agent360/plugins/wp-toolkit.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360/plugins/yum-updates.py` & `agent360-1.2.44/agent360/plugins/yum-updates.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360-example.ini` & `agent360-1.2.44/agent360-example.ini`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/agent360.egg-info/PKG-INFO` & `agent360-1.2.44/agent360.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent360
-Version: 1.2.43
+Version: 1.2.44
 Summary: 360 agent
 Home-page: https://github.com/plesk/agent360
 Author: 360
 Author-email: 360support@webpros.com
 Maintainer: 360
 Maintainer-email: 360support@webpros.com
 License: BSD-3-Clause
```

### Comparing `agent360-1.2.43/agent360.egg-info/SOURCES.txt` & `agent360-1.2.44/agent360.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agent360-1.2.43/setup.py` & `agent360-1.2.44/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     install_requires = ['psutil==5.6.7', 'netifaces', 'configparser==3.5.0', 'future']
 else:
     install_requires = ['psutil', 'netifaces', 'configparser', 'future']
 
 
 setuptools.setup(
     name='agent360',
-    version='1.2.43',
+    version='1.2.44',
     description='360 agent',
     long_description_content_type='text/markdown',
     long_description=readme,
     url='https://github.com/plesk/agent360',
     author='360',
     author_email='360support@webpros.com',
     maintainer='360',
```

