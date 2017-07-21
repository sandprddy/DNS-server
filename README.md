# DNS-server
A python regular-expression based DNS server!

    USAGE:
    ./dns.py [-h] -c Config path [-i interface IP address]

The dns.conf should be set the following way:

    [RECORD TYPE CODE] [python regular expression] [answer]


Supported Request Types
=======================
    - A
    - AAAA
    
Round-Robin
===========
Round-robin rules are implemented.  Every time a client requests a matching rule, DNS will serve out the next IP in the list of IP's provided in the rule.  
A list of IP's is comma-separated.

