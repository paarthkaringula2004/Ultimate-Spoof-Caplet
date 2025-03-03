## Install TP-Link Archer AC600 Driver on Kali Linux

### **Step 1: Update Your System**
```bash
sudo apt update && sudo apt upgrade -y
```

### **Step 2: Install Kernel Headers**
```bash
sudo apt install linux-headers-$(uname -r) -y
```

### **Step 3: Install the Realtek RTL88XXAU Driver**
```bash
sudo apt install realtek-rtl88xxau-dkms -y
```

### **Step 4: Reboot Your System**
```bash
sudo reboot
```

### **Step 5: Check If the Adapter is Detected**
```bash
iwconfig
```
OR  
```bash
ip a
```

### **Step 6: (If Not Working) Manually Load the Module**
```bash
sudo modprobe 88XXAU
```

### **Now Your TP-Link Archer AC600 Should Work on Linux! 🚀**
