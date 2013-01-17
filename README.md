nmap-to-fo
===============

Conver nmap XML directly in to XML-FO

This xsl file will convert the output of nmap -oX directly into usage XML-FO that can be easily converted into pdfs

Installation
===============

*Latest version: [https://github.com/tilikammon/nmap-to-fo]

Dependencies
===============

To convert the outputed xml file into a working pdf fop version 1.1rc1 from:

[http://apache.mirrors.pair.com/xmlgraphics/fop/binaries/fop-1.1rc1-bin.zip]

Usage
==============

1. run nmap with -oX flag for xml output
    $ nmap -oX ./nmap.scan.xml localhost

2. convert output xml to pdf using the above xsl file
    $ fop -xml nmap.scan.xml -xls nmap_fo.xsl -pdf nmap.scan.pdf

