requirements (2 swithches , 2 Pc) and connect pc 1 by sw1 and connect pc2 by sw2
then connet 2 sw 
and config  2 pc by add ip manual 
then config every switch 
command in sw1
-----------------
>en
conf t
hostname sw1
interface vlan 1
ip address 10.0.0.x 255.255.255.0
no shutdown
exit 
interface range fa0/1 -3
channel group 1 mode active 
exit
exit
show etherchannel summary
show ip enterface brief
--------------------
command in sw 2
>en
conf t
hostname sw2
interface vlan 1
ip address 10.0.0.x 255.255.255.0
no shutdown
exit 
interface range fa0/1 -3
channel group 1 mode active 
exit
exit
show etherchannel summary
show ip enterface brief
--------------------------
