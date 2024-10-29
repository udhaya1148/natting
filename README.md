# Natting - MASQUERADE
  Masquerade helps to share internet one system to another system
## Install iptables-persistent
```
sudo apt install iptables-persistent
 ```
## natting command
```
sudo iptables -t nat -A POSTROUTING -o <wifi interface name or interface which have internet connection -j MASQUERADE
```
## Save natting config
```
sudo iptables-save
```
# Save permanent natting conig 
## switch user to root
```
  sudo su - 
```
## save command
```
iptables-save >> /etc/iptables/rules.v4 
iptables-save
```
## natting list
```
sudo iptables -t nat -L
```
## set ip address, gatewave, subnet to wired interface
