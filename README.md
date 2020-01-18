# Nmap

When scanning a subnet for auditing purposes run the following:
 
                 nmap -A -v -oA "$(date +%T)_nmap_scan" <IP Address/CIDR>
 
For other scan types, see the nmap cheatsheet in the additional resources section.

To transform the xml output of the previous command into an html document, run the following:

                  xsltproc path/to/nmap.xsl path/to/nmapscan.xml > nmapscan.html

If xsltproc is not installed, run the following:
       
       Debian:   sudo apt-get install -y xsltproc
       CentOS:   sudo yum install libxslt

Nmap XSL file can be downloaded by running:

                   git clone https://github.com/dbarr914/Nmap.git
