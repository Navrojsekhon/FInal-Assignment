# **Standard Operating Procedure (SOP)**
## **Setting Up a Wi-Fi Network at Home**

---

## **1. Title**
**SOP for Setting Up a Home Wi-Fi Network**

---

## **2. Approval Table**
| Role | Name |  Date |
|------|------|-------|
| Document Author | Navroj Sekhon | 2025-11-24 |
| Reviewer | Simranjit Kaur | 2025-11-24 |
| Second Reviewer | Temilade | 2025-11-24 |
| Approver | Anshveer Singh | 2025-11-24 |

---

## **3. Reversion History**
| Version | Date | Author | Changes |
|---------|--------|----------|----------------|
| 1.0 | 2025-11-22 | Navroj Sekhon | Initial SOP created |
| 1.1 | 2025-11-23 | Simranjit Kaur | Improved structure and steps |
| 1.2 | 2025-11-24 | Anshveer Singh | Added visuals section |
| 1.3 | 2025-11-24 | Temilade | Final touch |

---

## **4. Purpose**
This SOP gives step-by-step instructions and rationale for installing, configuring, securing, and verifying a home Wi-Fi network. 
Use it when installing a new router, replacing an existing device, or onboarding someone who will maintain the network.
This ensures consistent installation, proper configuration, and secure wireless access for all home devices.

---

## **5. Scope**
This SOP applies to:
- Home users installing Wi-Fi for the first time  
- Users setting up a new router or upgrading equipment
- Users replacing or upgrading existing home Wi-Fi equipment  

It covers:
- Unboxing and physical connections.
- Router admin access and configuration.
- Security hardening (passwords, encryption, guest network).
- Basic performance and coverage checks.

---

## **6. Responsibilities**
| Task | Responsible Person |
|------|-------------------|
| Select Wi-Fi equipment | Navroj Sekhon |
| Install router & connect modem | Simranjit Kaur|
| Configure Wi-Fi & security | Anshveer Singh |
| Verification of setup | Temilade |

---

## **7. Required Equipment**
- Wireless Router - ensure it supports current Wi-Fi standards (at least Wi-Fi 5; Wi-Fi 6 preferred)
- Modem (Provided by ISP) - provided by ISP or a compatible third-party modem. 
- Ethernet Cable - Cat5e or Cat6 recommended
- Power Adapter - for router and modem 
- Laptop -  to access router settings and perform tests 

---

# **8. Step-by-Step Guide**

---

## **Step 1: Unbox the Router**
1. Open the package and remove: router, power adapter, Ethernet cable(s), quick start guide.
2. Inspect for damage and confirm included items match the packing list.
3. Note the router’s model, default SSID, default admin username, and default password printed on the label or quick guide.

  ![1](https://github.com/user-attachments/assets/96a92428-4a63-4945-8092-362d1f71df64)


**Purpose:** It Ensures that all required hardware for setting up the network is available before configuration.

---

## **Step 2: Connect Router to Modem**
1. Power off the modem (if present).
2. Connect one end of the Ethernet cable to the modem’s LAN (or the ISP port) and the other end to the router’s WAN/Internet port.
3. Power on the modem, wait until it finishes initializing (LEDs stable).
4. Plug in and power on the router; wait for it to boot (status LED indicates ready).

<img width="721" height="306" alt="2" src="https://github.com/user-attachments/assets/9dffd539-a42c-45d2-af45-b52dcac1af37" />


**Purpose:** It Delivers the internet signal from the modem to the router so it can broadcast Wi-Fi.

---

## **Step 3: Access Router Settings**
1. Connect a laptop to the router using Ethernet (recommended for initial config).
2. On Windows: Open Command Prompt and run `ipconfig` to find the **Default Gateway** address (the router IP).
3. Open a browser and enter the Default Gateway (commonly `192.168.0.1`, `192.168.1.1`, or `192.168.1.254`).
4. Log in using the default admin credentials printed on the device label.

<img width="464" height="500" alt="3" src="https://github.com/user-attachments/assets/e887a1e2-3420-466f-a470-f5fc9ae0fbed" />

<img width="959" height="473" alt="51" src="https://github.com/user-attachments/assets/be845eec-10ee-469b-863f-942044eb5284" />




**Purpose:** Accessing the admin interface allows configuration of Wi-Fi and security settings.

---

## **Step 4: Set Wi-Fi Network Name (SSID)**
1. Go to **Wireless Settings**.  
2. Change the SSID to a recognizable name but not personally identifying(Example: *DRDANGER*).
3. If router supports dual/tri-band, create separate SSIDs for each band if desired (e.g., `DRDANGER-2G` and `DRDANGER-5G`)

<img width="959" height="470" alt="53" src="https://github.com/user-attachments/assets/f2ce71a4-1cd9-4537-8ad6-bcd044100e54" />




**Purpose:** Clear SSIDs help family members identify networks; separating bands helps devices choose between range (2.4 GHz) and speed (5 GHz).

---

## **Step 5: Set a Strong Password**
1. Under wireless security, select **WPA2-Personal** or **WPA3-Personal** if supported. **Avoid WEP and WPA (TKIP) — they are insecure.**
2. Create a **Wi-Fi passphrase** that is more secure(12+ characters, mixture of upper/lowercase, numbers, symbols).

![6](https://github.com/user-attachments/assets/d9d77d70-5fc8-48d3-b3ea-dd8743c65414)



**Purpose:** This will protect the network from unauthorized access. Default admin credentials are widely known and present a major security risk.

---

## **Step 6: Optional Advanced Settings**
- **Guest Network:** Create an isolated SSID for visitors that restricts access to your internal LAN devices (printers, NAS). Use WPA2/WPA3 and set an expiration or password you can change easily.
- **MAC Address Filtering:** Adds administrative control but is not an effective security measure by itself (MACs can be spoofed). Use only as an additional control.
- **QoS (Quality of Service):** Prioritize traffic for devices or applications (e.g., VoIP, gaming, video conferencing).
- **Parental Controls:** Schedule or block specific websites/services per device.
- **VLANs:** Segment devices (e.g., IoT devices on a separate VLAN) if router supports it.
- **Remote Management:** Disable WAN-side remote admin unless necessary. If needed, restrict by IP and enable strong authentication.

<img width="959" height="472" alt="54" src="https://github.com/user-attachments/assets/ee5b880c-dd0d-4906-871e-4ccb05344e2b" />
<img width="959" height="467" alt="55" src="https://github.com/user-attachments/assets/05c20b9f-7786-4c49-bb26-9706ceed58cb" />
<img width="959" height="469" alt="56" src="https://github.com/user-attachments/assets/607ab9c6-ab8a-4b5b-996e-ee913cffe5b0" />


**Purpose:** Improves security and stability based on user needs. Advanced controls also improve performance and management when used properly.

---

## **Step 7: Save Settings & Restart Router**
1. Click **Save/Apply** after changes.
2. Perform a controlled restart from the admin interface (or power cycle).
3. Confirm settings persist after reboot.

![15](https://github.com/user-attachments/assets/c4e24f05-301c-404e-8664-8e8e31bd7d24)



**Purpose:** A restart ensures all services reload with new settings. Confirming persistence prevents surprises later.

---

## **Step 8: Connect Devices**
1. On each device (laptop, phone, smart TV), open Wi-Fi settings and select your SSID.
2. Enter the Wi-Fi passphrase you configured.
3. Optionally, configure static IPs for devices that need persistent addresses (e.g., printers, NAS) using DHCP reservation where possible.

<img width="732" height="460" alt="5" src="https://github.com/user-attachments/assets/f8edd9e9-d9c9-45a2-abf3-4e5c0ed00df3" />


**Purpose:** It confirms that Wi-Fi network is working correctly.

---

## **Step 9: Test Connectivity**
1. Open a browser and load several websites to verify internet access.
2. Run an internet speed test (e.g., speedtest.net) from a few locations in the house to check throughput.
3. Walk test Wi-Fi coverage: check signal and performance in rooms where devices will be used.

  <img width="705" height="463" alt="10" src="https://github.com/user-attachments/assets/9fff19db-4d2d-406a-a1f0-45dd8bbe03d1" />


**Purpose:** Verifies service quality and coverage; identifies weak spots where an extender or repositioning is needed.

---

# **9. Visual of full model and explanation**

![11](https://github.com/user-attachments/assets/77e7bf36-7806-4a2e-9022-ec3ece6d028f)

This image shows a simple home Wi-Fi network layout:
- The Internet comes from your service provider.
- It first connects to a Modem, which converts the incoming signal.
- The modem connects to a Router.
- The Router creates the Wi-Fi network.
- Multiple devices like computers and phones connect wirelessly to the router to access the internet.\
**In short: Internet → Modem → Router → Devices.**

# **10. Security & Maintenance Checklist**
- Change admin password from defaults.
- Use WPA2/WPA3 with a strong Wi-Fi passphrase.
- Disable WPS and remote admin on WAN.
- Enable automatic firmware updates or check monthly for firmware releases.
- Regularly update device credentials (guest network password, admin password).
- Document network configuration and store in a safe place (model, firmware version, SSIDs used, static IPs, DHCP reservations).
- Backup router configuration (if supported) before major changes.
- Revoke or rotate guest credentials periodically.

# **11. Troubleshooting — Common Issues & Fixes**
- **No Internet after setup:** Verify modem is online (ISP light), check WAN IP on router; restart modem then router.
- **Cannot access router admin page:** Confirm Ethernet connection, verify gateway IP (`ipconfig` / `ip route`), clear browser cache or use a different browser/device.
- **Weak Wi-Fi signal:** Move router to central/high location, reduce obstacles, change channel, or add mesh/extender.
- **Devices won’t connect:** Reboot device, forget network and reconnect, check MAC filtering, confirm password correctness.
- **Intermittent drops:** Check for firmware update, reduce interference (microwave, cordless phones), test with different band.

# **12. Conclusion**
This SOP gives you a full, step-by-step guide on how to set up a safe and properly working Wi-Fi network at home. By following all the steps in the document, you can make sure that:
- Your Wi-Fi is installed correctly
- Your network is secure from unauthorized access
- All your home devices can connect smoothly and reliably\

In simple words, it ensures your home Wi-Fi is set up the right way, protected, and runs without problems.
