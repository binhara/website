---
layout: obsolete
title: "Mono:IA64"
lastmodified: '2006-05-22'
permalink: /old_site/Mono:IA64/
redirect_from:
  - /Mono:IA64/
---

Mono:IA64
=========

The IA64 port is at the same level as the x86/amd64 ports. Currently, only linux is supported.

The port was started by Zoltan Varga in May 2005 and completed in August of the same year.

Building Mono on IA64
=====================

In addition to the usual mono dependencies, it depends on the libunwind package to implement exception handling:

[http://www.hpl.hp.com/research/linux/libunwind/](http://www.hpl.hp.com/research/linux/libunwind/)

By default, the mono GC is configured to use 8KB pages, which will not work on IA64 machines with a 4KB page size. To check the page size on your system, type:

zcat /proc/config.gz | grep PAGE\_SIZE\_4KB

If this prints something like this:

CONFIG\_IA64\_PAGE\_SIZE\_4KB=y

then mono needs to be compiled with a compiler flag to use 4KB pages:

configure "CFLAGS=-DHBLKSIZE=4096"

A runtime compiled this way will work on machines using both 4KB and 8KB pages.

