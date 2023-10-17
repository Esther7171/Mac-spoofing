# spoofing mac address

# to view current mac address:
```bash
macchanger -s wlan0
```
* current mac addrs 
![Screenshot 2023-10-17 235833](https://github.com/Esther7171/spoofing-mac-address/assets/122229257/cabb223e-f9f5-4aa8-aa65-a6d15939a139)

# -----spoofing mac address -----
- down the interface 
```bash
ifconfig wlan0 down
```
*  (-r ) to generate random mac address
```bash
macchanger -r wlan0 
```
![Screenshot 2023-10-17 235855](https://github.com/Esther7171/spoofing-mac-address/assets/122229257/9342cc8a-496e-4b82-abeb-3ceec4b0757b)

* up the interface
```bash
ifconfig wlan0 up
```

# bring back to permananet mac address 
## there are 2 ways to get back permanent mac address

 * restart system
 ```bash
 init 6
 ```
## or
```bash
ifconfig wlan0 down
```
* (-p) for switch to permananet
```bash
macchanger -p wlan0  
```
![Screenshot 2023-10-17 235913](https://github.com/Esther7171/spoofing-mac-address/assets/122229257/bd41b34b-fc06-479a-b19e-72822cc222e6)

# 1. bypass blacklist
```bash
macchanger -r wlan0 
```
# 2. bypass whitelist
* (-m) to give what connected devie mac address
```bash
macchanger -m <mac address> wlan0
``` 
## 🚀 About Me
* still finding.

