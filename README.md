# ARP-Attack-and-Network-Sniffing
# Explore Network Sniffing and ARP Attacks

### AIM:

To explore network sniffing and ARP Attacks

### STEPS:

### Step 1:

Install Parrot Security OS either in a partition, VirtualBox or in live mode.

### Step 2:

Investigate the various categories of network security tools available in Parrot OS, such as:
* arpspoof
* dsniff
* Metasploit Framework
* Wireshark
* Ettercap
* tcpdump


### Step 3:
Open the terminal and execute some Parrot OS commands.

```bash
cat /etc/os-release
ip addr
ip route
ip neigh
ifconfig
```

### ARP Attacks:  
ARP spoofing is an attack in which an attacker sends forged ARP packets that associate the attacker's MAC address with the IP address of another computer on a local network.

Boot Parrot OS and Windows 7 virtual machines.

In Windows 7, open Command Prompt and execute:

```cmd
ipconfig
arp -a
```

### OUTPUT:
<img width="1024" height="765" alt="image" src="https://github.com/user-attachments/assets/fe942673-e155-4f94-ae40-40dd2a8c6405" />


From Parrot OS, identify the active network interface using:

```bash
ifconfig
```

### OUTPUT:
<img width="800" height="667" alt="Screenshot 2026-10-30 134800" src="https://github.com/user-attachments/assets/c23ee6ca-6946-4883-936b-6dfe3922b008" />


Examine the ARP neighbor table using:

```bash
ip neigh
```

### OUTPUT:
<img width="807" height="156" alt="Screenshot 2026-10-30 134815" src="https://github.com/user-attachments/assets/4aad0c74-3eb5-4933-92d2-cb7a0f5895d0" />


Check the routing information using:

```bash
ip route
```

### OUTPUT:
 <img width="782" height="130" alt="Screenshot 2026-10-30 134834" src="https://github.com/user-attachments/assets/6acf5e51-ad98-4704-a3ee-34b0a93686a0" />




 
ARP spoofing concepts and their effects on IP-to-MAC address mappings were studied in an isolated virtual network.

### dsniff:
dsniff is a collection of network auditing and traffic analysis tools used to examine network traffic.

Install dsniff using:

```bash
sudo apt update
sudo apt install dsniff -y
```

Check the available utilities using:

```bash
dsniff -h
dpkg -L dsniff
```

### OUTPUT:
<img width="726" height="667" alt="Screenshot 2026-10-30 135023" src="https://github.com/user-attachments/assets/dc27062d-1890-4378-adc7-9681341cbe8a" />

### Metasploit Framework:
Metasploit is a penetration-testing framework used for security testing and vulnerability assessment.

Open Metasploit using:

```bash
msfconsole
```

### OUTPUT:
<img width="721" height="662" alt="Screenshot 2026-10-30 135205" src="https://github.com/user-attachments/assets/4bad67c0-0cbb-471f-b9a2-eb687b03e6c2" />




Search for FTP-related auxiliary modules using:

```text
search type:auxiliary ftp
```

### OUTPUT:
<img width="805" height="601" alt="Screenshot 2026-10-30 135317" src="https://github.com/user-attachments/assets/06d307db-bf67-48a4-b8af-f57c0756c6e9" />
Examine FTP service identification modules.

### Wireshark:
Wireshark is a network protocol analyzer used to capture and examine network packets.

Invoke Wireshark using:

```bash
sudo wireshark
```
<img width="941" height="851" alt="Screenshot 2026-10-30 125530" src="https://github.com/user-attachments/assets/52cf00c2-0240-434c-b55f-d31626322d38" />


Examine the various menus, controls, packet details and protocol information available in Wireshark.

### OUTPUT:
<img width="1110" height="692" alt="image" src="https://github.com/user-attachments/assets/7903d4fa-5f00-4990-a220-bad3a305ac07" />

### ARP packet:
<img width="902" height="906" alt="image" src="https://github.com/user-attachments/assets/447b7477-f0a8-44b0-8078-a38f15e21436" />

### Ettercap:
Ettercap is a network security tool that supports active and passive network analysis and host discovery.

Open Ettercap using:

```bash
sudo ettercap -G
```


Explore the following menus:

*Sniff
*Hosts
*Targets
*View
*Plugins 


Examine the graphical interface and network analysis features.

### OUTPUT:
<img width="856" height="707" alt="Screenshot 2026-10-30 135415" src="https://github.com/user-attachments/assets/b3f7c8c7-fedd-41ec-baae-827cc2123db6" />




### tcpdump:
tcpdump is a command-line network packet analyzer used to capture and examine network traffic.

Check the installed version using:

```bash
tcpdump --version
```

Examine the available network interfaces using:

```bash
sudo tcpdump -D
```


### OUTPUT:
<img width="803" height="365" alt="Screenshot 2026-10-30 135537" src="https://github.com/user-attachments/assets/8378a236-0d60-4aae-a0d1-b76bea2c5c6e" />

Capture ARP packets on the active interface using:

```bash
sudo tcpdump -i enp0s3 arp
```


Stop packet capturing using Ctrl + C.

### OUTPUT:
<img width="492" height="175" alt="Screenshot 2026-10-30 135617" src="https://github.com/user-attachments/assets/6243a407-8290-44d1-95fa-98f9c084ea34" />
<img width="703" height="290" alt="Screenshot 2026-10-30 135642" src="https://github.com/user-attachments/assets/c8f0f179-192c-4011-8151-c62184918757" />


### RESULT:
Thus, the network security and network sniffing tools available in Parrot OS, including arpspoof, dsniff, Metasploit, Wireshark, Ettercap and tcpdump, were explored successfully. The concepts of ARP attacks, ARP tables, network interfaces and packet analysis were studied.
