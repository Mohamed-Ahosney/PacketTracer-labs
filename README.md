
![accesslist](https://github.com/user-attachments/assets/5cd955f7-08bb-4b25-ae2a-58e939c77d67)



access control list 
-------------------
In case any "SR IP" not exit in access control list "DENY"


IP ACL
         Standared                           Extended
numbered          named            numbered         named    
1-99                               100-199
1300-1999                           2000-2599
kol interface leeha acl list 1 only          
--------------------------------------------------------
standared
filter date based on source only 
-------------------------------------------------------
extended 
filter date based on src IP 
L3 or L4 ,L7 application
---------------------------------------------------
lab 1
en hostname 
lab2
give all interfaces ip and mask
and n shut down
lab 3/7/11
------------------
"ospf"
router ospf 1
network 0.0.0.0 255.255.255.255 area 0
show ip route ospf
-------------------
from madrid ping  on ab3d haga 
------------------------------

deny ping from madried and barclona 
lap12
madried# access list 100 deny icmp srcip wildcardmask , dist wiledcardmask
barchlona# access list 100 deny icmp srcip wildcardmask , dist wiledcardmask
access list 100 permit IP  any any 
--------------------
active 
interface g0/0
ip access group 100 in 

show access list 
then make ping 
------------------
from madried ping 4.4.4.1
from barclona ping 2.2.2.1
