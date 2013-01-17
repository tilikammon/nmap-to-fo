nmap-to-fo
===============

Conver nmap XML directly in to XML-FO

This xsl file will convert the output of nmap -oX directly into XML-FO that can be easily converted into pdfs

Installation
===============

* Latest version: [https://github.com/tilikammon/nmap-to-fo]

Dependencies
===============

To convert the outputted xml file into a working pdf use fop from:

[http://apache.mirrors.pair.com/xmlgraphics/fop/binaries]

Usage
==============

* Run nmap with -oX flag for xml output
	nmap -oX ./nmap.scan.xml localhost

* Convert output xml to pdf using the above xsl file with fop
	fop -xml nmap.scan.xml -xls nmap_fo.xsl -pdf nmap.scan.pdf

