---
layout:     post
title:      "yum安装jdk"
subtitle:   "yum安装jdk,本文以jdk1.8为例"
date:       2022-06-02 12:00:00
author:     "LiuYang"
catalog:    false
header-style: text
tags:
  - linux
  - jdk
---



1、查看是否安装jdk

	rpm -qa |grep java

2、已安装就批量卸载

	rpm -qa | grep java | xargs rpm -e --nodeps 

3、查找安装包

	yum search java-1.8.0-openjdk

4、安装

	yum install java-1.8.0-openjdk.x86_64 -y
	
5、查看是否安装成功

    java -version

注意：jdk默认安装路径：/usr/lib/jvm/,完整JAVA_HOME为：/usr/lib/jvm/jdk包名



