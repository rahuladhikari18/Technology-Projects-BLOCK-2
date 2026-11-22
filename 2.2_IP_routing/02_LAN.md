
# 2. Part B — Configuring the LAN

## 2.1 Static IP Configuration
### Pi A (192.168.50.1)
> Insert screenshot here

### Pi B (192.168.50.2)
> Insert screenshot here

## 2.2 Explanation
Explain:
- What is a static IP address?
 ANSWER : An IP address that is manually assigned to a device and does not normally change. It allows devices on a network to have fixed addresses so they can communicate with each other easily.
 
- Why both devices cannot use the same address
  ANSWER :Both devices cannot use the same IP address because it causes an IP address conflict. The network will not be able to identify which device should receive the data. This can cause connection problems and prevent devices from communicating properly. Every device on the same network must have a unique IP address.
   
- Why we use /24
 ANSWER :We use /24 to represent the subnet mask 255.255.255.0. It means that the first 24 bits of the IP address identify the network, while the remaining 8 bits identify individual devices.

