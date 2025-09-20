# CSR1000v

enable
config t
int g1
ip addr dhcp
no shut
exit

config t
logging on
logging host 208.8.8.133 transport udp port 9001
logging trap informational

sh ip int bri
do sh ip int bri

config t
int g2
no shut
