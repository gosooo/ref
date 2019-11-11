---
title: SYS ~~ Package Manager
description: A package manager or package-management system is a collection of software tools that automates the process of installing, upgrading, configuring, and removing computer programs for a computer's operating system in a consistent manner.
published: true
date: 2019-11-11T21:04:46.396Z
tags: packagemanager, yum, pacman, apt, dnf, 00-sys
---

# Header
Your content here



solved with:
vi /etc/yum.conf
    proxy=http://10.0.8.152:3128



HTTP Error 403 - Forbidden
CentOS Cannot Find a Valid Baseurl for Repo Base/7/x86_64

/etc/sysconfig/network-scripts/ifcfg-ens32

yum clean metadata
yum check-update
yum clean all
yum repolist all
yum repolist all | grep 'enabled'

/etc/yum.repos.d/CentOS-Base.repo

curl -v 'http://mirrorlist.centos.org/?repo=os&arch=x86_64&release=7'



mirrorlist=http://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=os&infra=$infra