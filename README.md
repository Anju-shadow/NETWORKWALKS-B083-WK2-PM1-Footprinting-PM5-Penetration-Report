**# NETWORKWALKS-B083-WK2-PM1-Footprinting-PM5-Penetration Testing-Report**
☑️Penetration Testing Report — Footprinting & Network Scanning

**📌 Project Information**

| 🧩 Component | ⚙️ Detail |
| :--- | :--- |
| Program | cybersecurity program at Networkwalks |
| Week | 02|
| ⚡ Module | W2-PM1 — Multiple Kali Tools|
|           | W2-PM5 — Zenmap Scanning |
| 🐉Phases Covered |Phase 1: 👣Reconnaissance & Footprinting  |                	
|           |Phase 2: Scanning & Network Discovery |
| 🌐 Target | Networkwalks |
|  Additional target | My own LAN network |
| 🔐Permission Secured | Yes |
| 🚪 Repository | Git hub |
------------------------------------------------
**1.Liability Desclaimer:**
-----------------

I have performed these activities only on systems and devices where I had secured written permission or on devices/systems that I own myself.

All materials are provided for educational and research purposes only. Do not use anything from this report to break the law.

The instructor, authors, and Networkwalks are not responsible for misuse of the information provided in this report. Every action taken using this knowledge is the user's own responsibility.

Unauthorized access to computer systems can result in criminal charges, financial penalties, loss of employment, and other legal consequences.


**2.Introduction:**
----------------------
This Report covers my Week 2 project where  the footprinting and scanning on a network of Networkwalks.com domain with written permission to perform the basic attacks in an isolated environment.Where:-
W2 -Module 1:-This module demonstrate footprinting phase by using Kali linux tools.

W2-Module 2:-Here It covers the scanning phase.

Together, they demonstrate how a security professional can move from gathering publicly available information to discovering live hosts on a network.

All commands were performed using Kali Linux for footprinting and a Windows PC with Zenmap installed for network scanning.

Each activity includes:

- Network reconnaissance
- Port scanning 
- Screenshot evidence collected
- Report maintaing
- Security tool experimentation with Zenmap

**3.⚙️Tools used:**
---------------------
| 🧩 Tools |  Aim |                                                                                                           
| :--- | :--- |
| 🖥️ Kali Linux & windows OS | OS used for recognaissance and scanning |
| 🧠 WHOIS |Shows Public available domain registeration details ,date,server name.  |
|  🌐 WHATWEB |  Fingerprint web technologies such as servers, CMS platforms, plugins, and IP information|
| 🧠 Nslookup | Domain name to ip address using DNS |
| ✴️Curl-I  | Inspect HTTP response headers from a website |
| 📡 Wafw00f | Inspect Firewall used in web application |
 | DNSRecon |Enumerate DNS records such as NS, MX, SPF, TXT, and SRV records|
| Zenmap (N-map GUI) |Scan the local subnet to identify live hosts, IP addresses, and MAC addresses |
| Windows CMD |  Information about local ip address and mac address |

**4.Activities Performed:**
------------------------------
**4.1 Footprinting & Reconnaissance**
------------------
I have performed footprinting on website Networkwalks.com domain using 6 Kali linux tools:-
- WHOIS
- WhatWeb
- Nslookup
- Curl-I
- Wafw00f
- DNSRecon
Each tools gave different details about the website.
---------------------------------
**WHOIS**
-----
Firstly of all,I used this tool to determine the Publicaly available details of domain like regesteration info.,server name,Date.

**WhatWeb**
------
Secondly I used this to fetch the Tech-service it used .And it gave me result like:-
- WordPress 7.0.4
- WP Download Manager 3.3.58
- Other information exposed by the website
  
  **Nsllokup**
  ----------
  Nslookup change domain name into ip address ,The ip address i got is:-

  **Curl**
  -----------
   used Curl with the **-I **option to inspect the HTTP response headers. This provided additional information about the web application
   and exposed the WordPress REST API endpoint /wp-json/.

  **Wafw00f**
  -------
  It is graphical firewall detector to detect that which firewall is used to protect the website.
  It gave result about the firewall used in website --> ModSecurity (SpiderLabs).
  
  **DNSRecon**
  ------
  Finally, I used DNSRecon to enumerate DNS records. The results provided information related to name servers, mail servers, SPF/TXT records, service records, and DNS software information.
  
  ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **4.2 Network Scanning with Zenmap**
  ------
For the second activity, I used Zenmap to perform network discovery on my local network. The scan required me to identify my local IP address and subnet, discover live hosts, identified their IP and MAC addresses, and generate a network topology.

I first used the Windows ipconfig command to identify my local IP address and LAN subnet,then entered the subnet into Zenmap and selected Ping Scan to identify active hosts.



