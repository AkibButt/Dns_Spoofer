# Dns_Spoofer
How to Use DNS spoofer.
Make sure you have installed all labries Like netfilterqueue and scapy.
Step1: Be man in the middle using arpspoofer.py
Step2: Use iptables -i FORWARD -j
 NFQUEUE --queue-num 0. #for capturing packet in queue so that u can modify packet and send user from 1 request to other
 If you use above attack to your local computer use
 
 iptables -i INPUT -j NFQUEUE --queue-num 0.
 #in this case we are using bing.com will be redirected to localhost webpage.
