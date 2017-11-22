Blockasn
===================

blockasn is a python script that places iptables blocks of prefixes belonging to specified autonomous systems. It fetches the prefix data from stat.ripe.net using their public api. 


Usage example:
-------------
ASN 32934 belongs to facebook. peeringdb.net and stat.ripe.net are good places to find the ASN of the organization you are attempting to block. 
```
Firewall /home/user/blockasn # ./blockasn 32934
<> Requesting IP prefix data for ASN 32934 from stat.ripe.net...
[+] Adding 73 IPv4 prefixes originated by ASN 32934
[+] Adding 13 IPv4 prefixes transitting ASN 32934
[+] Adding 130 IPv6 prefixes originated by ASN 32934
[+] Adding 23 IPv6 prefixes transitting ASN 32934

