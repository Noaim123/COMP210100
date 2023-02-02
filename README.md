#!/bin/bash

#FQDN
fqdn=$(hostname -f)

#OS name and version
info=$(hostname -I | grep -v "^127.")

#Root filesystem space
rfs=$(df -h | grep "/s")

#print output
echo "FQDN: $fqdn"
echo "OS:$info"
echo "IP address: $ipadd"
echo "Rfs: $rfs"
