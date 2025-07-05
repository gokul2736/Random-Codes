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




## profile changes

#### 🔧 Frameworks & Tools  
![Prototyping](https://img.shields.io/badge/Prototyping-FF6347?style=flat&logo=figma&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat&logo=django&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat&logo=flask&logoColor=white)
![Fernet](https://img.shields.io/badge/Fernet-007ACC?style=flat&logo=python&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=flat&logo=visualstudiocode&logoColor=white)
![Windows OS](https://img.shields.io/badge/Windows%20OS-0078D4?style=flat&logo=windows&logoColor=white)  
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat&logo=selenium&logoColor=white)
![VirtualBox](https://img.shields.io/badge/VirtualBox-183A61?style=flat&logo=virtualbox&logoColor=white)
![OCR Tesseract](https://img.shields.io/badge/OCR%20Tesseract-000000?style=flat&logo=tesseract&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white)
![React.js](https://img.shields.io/badge/React.js-61DAFB?style=flat&logo=react&logoColor=black)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white)  
![Fusion 360](https://img.shields.io/badge/Fusion%20360-FF6A00?style=flat&logo=autodesk&logoColor=white)
![OBS Studio](https://img.shields.io/badge/OBS%20Studio-100000?style=flat&logo=obs-studio&logoColor=white)
![Audacity](https://img.shields.io/badge/Audacity-000000?style=flat&logo=audacity&logoColor=white)
![Sony Alpha](https://img.shields.io/badge/Sony%20Alpha-000000?style=flat&logo=sony&logoColor=white)




![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
