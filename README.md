# Cybersecurity-2
NETWORK TRAFFIC ANALYSIS

Several customers of clients reported that they were not able to access the client company website www.yummyrecipesforme.com, and saw the error __“destination port unreachable”__ after waiting 
for the page to load. 

__I am tasked with analyzing the situation and determining which network protocol was affected during this incident.__ To start, I attempt to visit the website and receive the error
“destination port unreachable.” To troubleshoot the issue, I load my __network analyzer tool, tcpdump__, and attempt to load the webpage again. To load the webpage, my browser sends a query
to a DNS server via the UDP protocol to retrieve the IP address for the website's domain name; this is part of the DNS protocol. my browser then uses this IP address as the destination IP for
sending an HTTPS request to the web server to display the webpage. The analyzer shows that when i send UDP packets to the DNS server, __I receive ICMP packets containing the error message: 
“udp port 53 unreachable.”__

