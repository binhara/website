---
layout: obsolete
title: "Command Line MoMA"
lastmodified: '2008-03-14'
permalink: /old_site/Command_Line_MoMA/
redirect_from:
  - /Command_Line_MoMA/
---

Command Line MoMA
=================

Beginning with version 1.9 of [MoMA]({{site.github.url}}/old_site/MoMA "MoMA"), you can now run MoMA without showing a GUI. This is helpful for people who wish to add MoMA scans to their automated builds. For example, you may have a policy that only Mono supported methods should be used in your application.

To run MoMA from the command line, use:

``` bash
MoMA.exe --nogui C:\app\myapp.exe
```

If you have several assemblies to scan, you can enter them all:

``` bash
MoMA.exe --nogui C:\app\myapp.exe C:\app\myapp.dll C:\app\myapp2.dll
```

If you want to specify where the output report goes:

``` bash
MoMA.exe --nogui --out C:\app\momareport\report.html C:\app\myapp.exe
```

 If you encounter bugs, or need additional functionality, you can file a bug in Mono -\> Mono: Tools -\> MOMA category of bugzilla. See [Bugs]({{site.github.url}}/old_site/Bugs "Bugs").

