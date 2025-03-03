# Basic Spoofing Caplets  

🚀 **Basic Spoofing** contains lightweight **Bettercap caplets** for network spoofing, MITM attacks, and reconnaissance. These caplets provide fundamental **ARP spoofing, DNS spoofing, and SSL stripping** techniques for network penetration testing.  

---

## 📌 Caplets Overview  

### **1. BasicSpoof.cap**  
- Performs **ARP spoofing** to intercept network traffic.  
- Redirects packets through the attacker's machine.  
- Can be used for basic **MITM attacks**.  

### **2. hstshijack.cap**  
- Hijacks **HSTS-enabled websites** to downgrade HTTPS to HTTP.  
- Useful for SSL stripping and credential harvesting.  
- Works in combination with **SSLStrip** and **HTTP Proxy**.  

---

## 🛠️ How to Use  

### **Clone the Repository**  
```sh
git clone https://github.com/paarthkaringula2004/Ultimate-Spoof-Caplet.git
cd Ultimate-Spoof-Caplet/BasicSpoofing
```

### **Run in Bettercap**  
```sh
sudo bettercap -caplet BasicSpoof.cap
```
And after the Successful Step
```sh
sudo bettercap -caplet hstshijack.cap
```

---

## ⚠️ Disclaimer  
This project is for **educational & penetration testing purposes only**. **Unauthorized use is illegal** and may violate **cybersecurity laws**.  

---

📌 **Contributors & Support**  
👤 Created by **[@paarthkaringula2004](https://github.com/paarthkaringula2004)**  

Feel free to **fork, modify, and contribute**! 🚀  
