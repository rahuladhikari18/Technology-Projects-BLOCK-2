
## 🛠️ 3. Server Configuration (DHCP + DNS)

### 3.1 Static IP Settings  
To configure the server's static IP, navigate to the network adapter properties on the server OS (or configuration CLI in Cisco Packet Tracer), select IPv4 properties, and assign a permanent IP address (e.g., ⁠192.168.1.10⁠), a matching subnet mask (e.g., ⁠255.255.255.0⁠), the default gateway (e.g., ⁠192.168.1.1⁠), and the preferred DNS server address.  
 And then , Open the command prompt and run ⁠if configuration ⁠ (Windows) to confirm that the static IP, subnet mask, and gateway are applied correctly without conflicts.

📸 **Screenshot: Server IP configuration**

---

### 3.2 DHCP Configuration  
 The DHCP pool was configured by specifying the network scope parameters to automatically lease IP addresses to client devices. This included setting a starting IP address (e.g., ⁠192.168.1.100⁠), an ending address to define the pool size, the subnet mask, the default gateway address, and the DNS server IP address.  
 Afterthat, Connect a client PC to the network, set its IP configuration to "DHCP" (Automatic), and run ⁠ipconfig to verify that it successfully receives an IP address within the defined pool range along with the correct gateway and DNS settings.

---

### 3.3 DNS Configuration  
 The DNS service was enabled on the server to translate human-readable domain names into numerical IP addresses. Forward lookup zones were created, and specific A records (Host records) were added to map domain names (e.g., ⁠labserver.local⁠) to the server's static IP address.  
 Moreover, Open a terminal or command prompt on a client machine and use the ⁠nslookup [domain-name]⁠ command to check if the name successfully resolves to the correct server IP address.

📸 **Screenshot: DNS service + name entries**

