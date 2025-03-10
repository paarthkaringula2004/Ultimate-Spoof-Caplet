# Ultimate & Basic Spoof Caplets  

This repository contains **two sets of Bettercap caplets**:
- **Basic Spoofing Caplets** (for learning & understanding spoofing techniques)
- **Ultimate Spoof Caplet** (for advanced penetration testing & real-world attack simulations)  

---

## When to Use Which Caplet?  

### **1. Basic Spoofing Caplets** (Recommended for Learning)  
🔗 Location: `BasicSpoofing/`
- Helps understand **ARP spoofing, DNS spoofing & SSL stripping**.
- Ideal for **educational purposes** & understanding network vulnerabilities.
- Use it to **see how spoofing works** but without causing harm.

### **2. Ultimate Spoof Caplet** (Use with Caution)  
🔗 Location: `UltimateSpoof.cap`
- **Use only when required** (for ethical hacking & security testing).
- Designed for **serious penetration testing & security research**.
- Can cause **network disruptions** or **illegal activity if misused**.
- Always ensure **you have permission** before using this caplet.

---

## Precautions Before Using **Ultimate Spoof**  
🛡️ Follow these steps to stay secure & undetected:

1. **Use a compatible WiFi adapter**  
   Recommended: **TP-Link Archer T2U Plus (AC600)**
   
   ![Recommended WiFi Adapter](https://github.com/paarthkaringula2004/Project-Images-Video/blob/main/Images-Videos/Ultimate-Spoof-Caplet/tp-link-adapter.jpg)
 
   - [Amazon India](https://www.amazon.in/tp-link-archer-t2u-plus/s?k=tp+link+archer+t2u+plus)  
   - [Flipkart](https://www.flipkart.com/tp-link-archer-t2u-plus-ac600-high-gain-wireless-dual-band-usb-adapter/p/itm78f701f57c630)  
   - [TP-Link Official Store](https://www.tp-link.com/in/home-networking/high-gain-adapter/archer-t2u-plus/)


3. **Change the MAC Address:**  
   ```sh
   sudo ifconfig wlan1 down  
   sudo ifconfig wlan1 hw ether 00:11:22:33:44:55  
   sudo ifconfig wlan1 up  
   ```
4. **Enable Monitor Mode:**  
   ```sh
   sudo airmon-ng check kill  
   sudo ifconfig wlan1 down  
   sudo iwconfig wlan1 mode monitor  
   sudo ifconfig wlan1 up  
   ```
5. **Run in a controlled environment** (such as a test lab, not a public network).
6. **Ensure you have proper authorization** before performing any tests.
7. **Monitor your network activity** to avoid unintended damage.
8. **Stop all attacks immediately** if you notice instability or unintended impact.

---


### **Run Basic Spoofing Caplets**  
```sh
sudo bettercap -caplet BasicSpoof.cap
```
**With**
```sh
sudo bettercap -caplet hstshijack.cap
```
**And Use If Needed (Enable Packet Forwarding)**
```sh
echo 1 | sudo tee /proc/sys/net/ipv4/ip_forward
```


### **Run Ultimate Spoof Caplet**  
```sh
sudo bettercap -caplet UltimateSpoof.cap
```

---

## ⚠️ Legal Disclaimer  
This project is strictly for **educational & ethical penetration testing purposes only**. **Unauthorized use is illegal** and can lead to severe legal consequences. **Use responsibly!**  

---

📌 **Contributors & Support**  
👤 Created by **[@paarthkaringula2004](https://github.com/paarthkaringula2004)**  

Feel free to **fork, modify, and contribute**! 🚀  
