NOTE: This is a copy of source code which is available at http://code.google.com/p/ebcode/. Since the source code is available in download-only version, I decided to extract it and add to Git repository for easy online browsing in educational purposes. Below you can see original description of the project:

EveryBlock.com is an experimental news Web site that provides information at a "microlocal" level — by neighborhood or city block. It was funded by a grant from Knight Foundation, which requires the site's backend code to be open-sourced. Here is the code.

Overview
========

In an effort to make the code useful to as many people as possible, we've split it into several packages:

* The main package (probably the thing you're looking for) is the publishing system, known as ebpub.
* Second, the packages ebdata and ebgeo contain Python modules for processing data and making maps.
* Third, the packages ebinternal and everyblock round out the code that powers EveryBlock.com. They're internal tools and are likely not of general use, but we're including them to be complete.
* Finally, ebblog and ebwiki are our blog and wiki software, respectively. Because, dammit, the world needs another Django-powered blogging tool.

Things you should know
======================

We're excited to make this code available to you, but there are a few Important Things you should know about using it:

TRADEMARKS — In using this code, you may not call your product "EveryBlock." Of course, we would love it if you said it's inspired by EveryBlock, uses EveryBlock's code, etc., but you can't call it EveryBlock.

LICENSE — This code is Copyright 2007-2009 EveryBlock LLC and is made available to you under the GNU General Public License (GPL) version 3. To paraphrase, this means that if you distribute any changes, you must make them available under the same open-source license. Our documentation is licensed separately, under the Creative Commons Attribution-Share Alike 3.0 United States License. The Knight Foundation folks have requested we use these licenses.

DESIGN/UI — This code includes basic HTML templates, but the design ("look and feel") of EveryBlock.com is copyrighted and belongs solely to EveryBlock.com.

LANGUAGES/FRAMEWORKS — This code is written in Python, using the Django Web framework. It requires PostgreSQL and PostGIS.

Mailing list
------------
This code is being made available to you with no promise of support, but you might want to connect with other people using it on the ebcode mailing list.

ebpub
-----
Publishing system that powers EveryBlock.com.

Dependencies among packages: Requires ebgeo
ebdata
------
Various data-acquisition modules and scripts.

Dependencies among packages: Requires ebgeo, ebpub
ebgeo
-----
Various geographic/mapping utilities used by ebpub but packaged for optional standalone use.

Dependencies among packages: None
ebinternal
----------
Code for internal EveryBlock tools. Likely not of general use.

Dependencies among packages: Requires everyblock
everyblock
----------
Python package of code that is specific to EveryBlock.com, as opposed to the generic ebpub system. Likely not of general use.

Dependencies among packages: Requires ebgeo, ebpub, ebdata
ebblog
------
A Django-powered blog system used by the EveryBlock Blog.

Dependencies among packages: None
ebwiki
------
A Django-powered wiki used internally by EveryBlock.

Dependencies among packages: None
