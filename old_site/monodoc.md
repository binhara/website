---
layout: obsolete
title: "Monodoc"
lastmodified: '2006-12-16'
permalink: /old_site/Monodoc/
redirect_from:
  - /Monodoc/
---

Monodoc
=======

Monodoc is a set of libraries and applications for viewing and editing Mono class library documentation. Monodoc is part of the [Mono Documentation Project]({{site.github.url}}/old_site/Documentation "Documentation").

<table>
<col width="100%" />
<tbody>
<tr class="odd">
<td align="left"><h2>Table of contents</h2>
<ul>
<li><a href="#viewing-the-documentation">1 Viewing The Documentation</a>
<ul>
<li><a href="#the-gtk-documentation-browser">1.1 The Gtk# Documentation Browser</a></li>
<li><a href="#online-documentation">1.2 Online Documentation</a></li>
<li><a href="#mod-command-line-documentation-viewer">1.3 Mod (Command-Line Documentation Viewer)</a></li>
</ul></li>
<li><a href="#creating-documentation-contributing">2 Creating Documentation, Contributing</a></li>
<li><a href="#my-documentation-in-monodoc">3 My Documentation in Monodoc</a></li>
</ul></td>
</tr>
</tbody>
</table>

Viewing The Documentation
=========================

The Gtk\# Documentation Browser
-------------------------------

The doc browser is part of the [mono-tools](/index.php?title=Mono-tools&action=edit&redlink=1 "Mono-tools (page does not exist)") package, avaliable from the [Downloads]({{site.github.url}}/old_site/Downloads "Downloads") page.

Once installed, you can launch it from the "Programing" section of the Applications menu, as shown in the image below, or by typing *monodoc* in a terminal window.

[![Gnome menu-monodoc-1.png]({{site.github.url}}/old_site/images/1/1d/Gnome_menu-monodoc-1.png)]({{site.github.url}}/old_site/images/1/1d/Gnome_menu-monodoc-1.png)

The browser lets you navigate through different types of documentation installed on your system. Usually, it shows the documentation of:

-   Core Framework API
-   Mono libraries
-   Novell libraries
-   C\# Language Specification
-   Compiler error reference

Depending on the libraries installed on your system it can show additionally:

-   Gnome libraries
-   Mozilla library
-   Monkeyguide (Mono guide)

Of course, more documentation sources can be added from installed libraries or from your own generated documentation as explained in [Generating Documentation]({{site.github.url}}/old_site/Generating_Documentation "Generating Documentation"). Also, from inside the browser, you can [contribute]({{site.github.url}}/old_site/Monodoc_Contributing "Monodoc Contributing") to the documentation of the Mono project.

Online Documentation
--------------------

You can view the complete documentation library online (only API documentation) at [http://www.go-mono.com/docs/](http://www.go-mono.com/docs/).

Mod (Command-Line Documentation Viewer)
---------------------------------------

To browse API documentation from a shell terminal, you can use the \`mod' command. Use it to lookup types, or see the members of a type. You get the same information as the Monodoc graphical application, but displayed in a text-only web browser.

To get all the types in a namespace:

``` bash
mod N:System
mod N:Gtk
```

To see the members of a type, run mod like:

``` bash
mod T:System.Collections.ArrayList
```

You can restrict the output to just members by adding `/M`:

``` bash
mod T:System.Collections.ArrayList/M
```

You can also use C, P, F, and E for constructors, properties, fields, and events.

To get one method, copy-and-paste the URL from the output in the above:

``` bash
mod 'M:System.Collections.ArrayList.ToArray(System.Type)'
```

Creating Documentation, Contributing
====================================

-   For information on how to document your own class libraries using monodoc, see [Generating Documentation]({{site.github.url}}/old_site/Generating_Documentation "Generating Documentation").
-   If you would like to contribute to the mono class library documentation (and we would love it if you did!), see [Monodoc Contributing]({{site.github.url}}/old_site/Monodoc_Contributing "Monodoc Contributing").

My Documentation in Monodoc
===========================

See the [assembler]({{site.github.url}}/old_site/Assembler "Assembler") page for a description how to add your documentation to monodoc permanently.

