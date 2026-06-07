Date - 7/6/26

DNS stands for domain name system. Instead of remembering complex ips for websites, dns was created.
example - tanmaydawande.tech

TLD - top level domain is the .tech, .com, .io part
gTLD - .online, .club, .website
ccTLD(country code) - .in, .ca, .co.uk

Second level domain - tanmaydawande is the sld

subdomain - hi.google.com
a subdomain is a separate address at the network level. A path is just a different page on the same address.
path example google.com/hi These are two different things.

DNS record types
'A' record - these resolve to ipv4 addresses
'AAAA' record - these resolve to ipv6 addresses
CNAME record - these records resolve to another domain name to work out the ip address. example:- tanmaydawande.tech/quizgenai resolves to quizgenaiapp.onrender.com. 
MX(mail exchanger) record - tells the internet which mail server the should recivve emails sent to the domain.
for example, cloudfare you can add a mx record in which if you mail to sayhi@tanmaydawande.tech, some other email id inbox will recieve the email. 
TXT record - it holds arbitrary text now used to verify 


What exactly happens when you make a dns request
 1) When you request a domain, our computer first checks the cache. If not found, it moves to 2
 2) It checks the recursive DNS server. It has a lot of cache and usually frequently accessed domains llive here. If a miss, it moves on.
 3) The root dns servers of the internet redirects you to the corret tld. .com websites etc are sorted. It refers to the TLD domain.
 4) tld servers hold where to find the nameserver for the domain. Each website has multiple nameservers
 