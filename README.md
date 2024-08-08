## natting
# Install iptables-persistent
```sudo apt install iptables-persistent ```
# natting command
```sudo iptables -t nat -A POSTROUTING -o wlp0s20f3 -j MASQUERADE```
# Save natting config
```sudo iptables-save```
## Save permanent natting conig 
# switch user to root
```sudo su - ```
# save command
```iptables-save >> /etc/iptables/rules.v4 ```
```iptables-save```
