# Active Directory Security Lab

## 📌 About This Project
This is a home lab I built to learn how Active Directory works, how Windows logs security events,  
and how attacks look from a defender’s point of view.  
The lab was inspired by the myDFIR Active Directory Series on YouTube.

---

## 🖥️ Lab Environment
This lab was created using VirtualBox and includes:

- **Windows Server 2022** – Active Directory Domain Controller  
- **Windows 10** – Domain-joined workstation  
- **Kali Linux** – Attacker machine  
- **Ubuntu Server** – Splunk log server  

---

## 🛠️ Tools Used
- **Splunk Enterprise**  
- **Splunk Universal Forwarder**  
- **Sysmon**  
- **Hydra** (used for RDP brute force testing — Crowbar was replaced due to compatibility issues)  
- **Atomic Red Team**  
- **VirtualBox**

---

## 📘 What I Did
- Installed and configured Active Directory  
- Created domain users and joined a Windows 10 machine to the domain  
- Installed Sysmon and forwarded logs to Splunk  
- Simulated an RDP brute force attack using Hydra on Kali Linux  
- Detected failed and successful login attempts in Splunk  
- Used Atomic Red Team to generate attack activity and check visibility  

---

## 🧠 What I Learned
- How Active Directory authentication works  
- How brute force attacks appear in Windows logs  
- How to investigate Event IDs **4625** (failed logon) and **4624** (successful logon)  
- How blue team investigation connects with attacker behavior  

---

## Screenshots
All screenshots for this project are available in the `/screenshots` folder of this repository.

---

## Disclaimer
This project was created in a safe home lab for learning purposes only.  
Crowbar was part of the original tutorial, but Hydra was used instead due to compatibility issues on modern Kali Linux.

