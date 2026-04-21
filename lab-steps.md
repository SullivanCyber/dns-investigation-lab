## Step 1: DNS Query using dig

Command:
dig internal.company.com

Result:
(Write exactly what you see)

Analysis:
-Did it resolve?
-Was there an IP?
-Any errors like NXDOMAIN?

Step: Hosts File Manipulation

Action:
Added manual entry in /etc/hosts

Result:
Domain resolved to incorrect IP (192.168.1.100)

Analysis:
This simulates DNS spoofing or local override attack
