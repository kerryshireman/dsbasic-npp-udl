DataStage BASIC User Defined Language for Notepad++
=================================================

Developed by [Kerry Shireman][kerry].

Original Solarized color scheme developed by Ethan Schoonover <mailto:es@ethanschoonover.com>.

Introduction
------------

The [IBM WebSphere DataStage BASIC][datastage] editor lacks, among other things, syntax highlighting.
[Notepad++][npp] 6.3 and later has a language definition feature named
[User Defined Language (UDL) 2.0][udl2].  This project implements UDL 2.0 for DataStage BASIC.
Three color schemes are included, two of which are based on the Solarized color palette by
Ethan Schoonover <mailto:es@ethanschoonover.com>.

For more information on Solarized, please visit the [Solarized home page][solarized] or the [Solarized repository][solarizedrepo].

**NOTE:** This project is a language-specific implementation of Solarized.  The Notepad++ Style Configurator already supports Solarized for its built-in languages.  If you're just interested in Solarized for Notepad++, please refer to its Style Configurator documentation.

Status
------
These UDLs were developed for DataStage BASIC v8.5, and to my knowledge are syntax complete.  If you run into issues, please open an Issue in the repository.

Requirements
------------
* [Notepad++][npp] 6.3 or later
* A few minutes for installation

Contents
--------
Three UDL color schemes are included in this distribution.

* DSB.xml - For an out of the box Notepad++ installation
* DSB-Solarized.xml - For those who prefer the Solarized theme
* DSB-Solarized-l.xml - For those who prefer the Solarized Light theme

Installation
------------
**Assumptions**

1. Notepad++ is installed on your machine

**All Installations**

1. Download this repository to your local filesystem, unarchive if necessary
2. In Notepad++, go to `Language | Define Your Language...`
3. Go to `Import...`, navigate to the appropriate UDL file (e.g. DSB.xml), click `Open`
4. Click the `X` button at top right, closing the dialog window

**Solarized Installations**

Another step is required to get the right background color for Solarized installations.

1. Go to `Setting | Style Configurator...`
2. Under `Language :` ensure that `Global Styles` is selected 
3. Under `Style :` ensure that `Global override` is selected 
4. Check the `Enable global background color` checkbox
4. Using the `Select theme` drop down, choose the appropriate theme (see table below for help):
5. Click `Save &amp; Close`

<table>
<caption>UDL to Theme</caption>
<tr>
<th>UDL</th>
<th>Theme</th>
</tr>
<tr>
<td>DSB-Solarized.xml</td>
<td>Solarized</td>
</tr>
<tr>
<td>DSB-Solarized-l.xml</td>
<td>Solarized-light</td>
</tr>
</table>


Usage
-----
The installed UDL will be invoked automatically when opening files with a ".dsb" extension.  ".dsb" isn't a DataStage BASIC convention; I just made it up during development.  If you have a file extension conflict, you may invoke the UDL on a file by file basis.  Here's how:

1. Go to `Language`, then click the installed language name near the bottom, e.g. `DSB` or `DSB-Solarized`.


Changing Themes
---------------
Notepad++ may become confused when two or more UDLs are associated with the same file extension.  If you already installed one of these UDLs and want to switch it out, follow these uninstallation steps **before** proceeding:

1. In Notepad++, go to `Language | Define Your Language...`
2. Click the `User language:` drop-down
3. Select the installed language (e.g. DSB, DSB-Solarized), then click `Remove`.
4. See the Installation section


Resources
---------

* [Solarized Color Scheme][solarized] by Ethan Schoonover
* [Notepad++][npp]
* [UDL 2.0 online documentation][udl2]
* [IBM InfoSphere DataStage - BASIC Reference Guide - v8.5][basicref]
* [IBM InfoSphere DataStage - Server Job Developer's Guide - v8.5][serverref]


Thanks
------

Many thanks to Ethan Schoonover for his awesome work on Solarized.

Thanks go to my colleague, Joy Stover, who encouraged me to get off my behind and do this.



[solarized]: http://ethanschoonover.com/solarized
[solarizedrepo]: https://github.com/altercation/solarized
[datastage]: https://www.ibm.com/software/data/infosphere/datastage/
[npp63]: http://notepad-plus-plus.org/download/v6.3.html
[npp]: http://notepad-plus-plus.org/
[udl2]: http://udl20.weebly.com/
[kerry]: https://github.com/haylo75
[basicref]: http://publibfp.boulder.ibm.com/epubs/pdf/c1898972.pdf
[serverref]: http://publibfp.boulder.ibm.com/epubs/pdf/c1898983.pdf