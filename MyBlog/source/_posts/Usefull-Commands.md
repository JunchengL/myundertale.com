---
title: Usefull Commands
date: 2019-04-12 23:03:20
tags:
  - Linux
categories: 
  - Linux
description: Some usefull commands in my work
---

# This post is to remind me of some usefull commands in my work.



## Disk Usage Analyse: 

~~~shell
df -hT 
~~~

~~~shell
du -sk ./* | sort -n
~~~


## Server swap to max capacity and need to free swap: 

~~~shell
swapoff -a && swapon -a
~~~

## Show files in order: 

~~~shell
Ls -ltr
~~~

## Catch key words with grep command: 

~~~shell
grep -ri 'proxy-internet' --exclude-dir=wp-content/uploads *
~~~

## Connexion in distance on Windows Server: 
MSTSC


## Change all files ownershipsr: 

~~~shell
chown -R ljckk:ljckk *
~~~

## Command in Vim: 
d G  ->delete full page

## Replace words with sed: 

~~~shell
sed -i -e "s/words_before_replacement/words_after_replacement/g" file.name
~~~

## Restart Apache gracefully: 
/etc/init.d/httpd reload

## Analyse ports: 
port 80 is listened?
~~~shell
netstat -auntp| grep 80
~~~

test port 80 on localhost 
~~~shell
nc -vz localhost 80
~~~
