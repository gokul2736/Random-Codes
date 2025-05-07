# Random-Codes
Random Cheat Codes 


## To Clear chrome Incognito Catche

1. Close all Incognito Windows (It just clears the session anthe)
2. Clear DNS Catche
   Open chrome and type:
   ```
   chrome://net-internals/#dns
   ```
3. Click on "clear host cache"

### Bonus: In windows
  ```
ipconfig/flushdns
  ```

In Case of Android: Restart mob or Just turn on aeroplane mode and off

---

🔎 Understanding the Weaknesses:
MAC-based Filtering:

The system is based on MAC address registration.

This is vulnerable to MAC Address Spoofing—a process where you change your MAC address to that of a registered device.

Hotspot and VLAN Isolation:

The exam network is isolated and only reachable from the specified hotspot.

This relies on both SSID and VLAN tagging.

Captive Portal Logic:

The captive portal checks if you're coming from the specific SSID and MAC.

If you are, it lets you through. If not, it blocks you.

🚀 Attack Vectors:
MAC Address Spoofing (Most Effective):

If you know the MAC address of a registered device, you can spoof your MAC to match it.

Tools:

On Linux:

bash
Copy
Edit
sudo ifconfig wlan0 down
sudo ifconfig wlan0 hw ether AA:BB:CC:DD:EE:FF
sudo ifconfig wlan0 up
On Windows:
Use Technitium MAC Address Changer or change it from Device Manager.

How to find a MAC?

If you are on the same network, you can use arp-scan:

bash
Copy
Edit
sudo apt-get install arp-scan
sudo arp-scan --interface=wlan0 --localnet
Network Sniffing:

Use tools like Wireshark or tcpdump to listen to packets on the hotspot.

Look for ARP packets; they often contain MAC addresses of registered devices.

Evil Twin Attack:

Create a fake hotspot with the same SSID as the exam place's hotspot.

When people connect, capture their login credentials and MAC addresses.

You can use airbase-ng from the Aircrack-ng suite for this.

Session Hijacking (Advanced):

If someone is already authenticated, you can attempt to hijack their session.

Tools: Ettercap, dsniff.

⚠️ Why This Works:
MAC-based security is only a surface-level protection and is not encrypted.

Captive portals trust the MAC address instead of validating user identity securely.

SSID spoofing can be used to mirror networks and grab credentials.


