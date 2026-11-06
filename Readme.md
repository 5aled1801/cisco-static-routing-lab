\# Cisco Packet Tracer – Multi-Router Static Routing



\## 📌 Project Overview



This project demonstrates a multi-router network topology built using \*\*Cisco Packet Tracer\*\*.



The main objective is to connect three different LAN networks through multiple routers using \*\*Static Routing\*\*, allowing devices in different networks to communicate with each other.



\## 🖥️ Network Topology



The network consists of:



\- 3 Routers

\- 3 Switches

\- 6 PCs

\- 3 LAN Networks

\- 1 Shared Inter-Router Network



\### Network Diagram



The topology connects three separate LANs through a shared transit network (`192.168.4.0/24`).



\## 🌐 IP Addressing Scheme



| Network | Network Address | Default Gateway |

|---|---|---|

| LAN 1 | 192.168.1.0/24 | 192.168.1.1 |

| LAN 2 | 192.168.2.0/24 | 192.168.2.1 |

| LAN 3 | 192.168.3.0/24 | 192.168.3.1 |

| Transit Network | 192.168.4.0/24 | N/A |



\### Router Interfaces



| Router | Interface IP | Connected Network |

|---|---|---|

| Router 1 | 192.168.2.1 | LAN 2 |

| Router 1 | 192.168.4.2 | Transit |

| Router 2 | 192.168.1.1 | LAN 1 |

| Router 2 | 192.168.4.3 | Transit |

| Router 3 | 192.168.3.1 | LAN 3 |

| Router 3 | 192.168.4.1 | Transit |



\## ⚙️ Technologies \& Concepts



\- Cisco Packet Tracer

\- IPv4 Addressing

\- Subnetting (/24)

\- Router Configuration

\- Static Routing

\- LAN Connectivity

\- Inter-Network Communication

\- Default Gateway Configuration

\- ICMP (Ping Testing)



\## 🔧 Configuration



Static routes are configured manually on each router using:



```bash

ip route \[destination-network] \[subnet-mask] \[next-hop]

```



Example:



```bash

ip route 192.168.1.0 255.255.255.0 192.168.4.3

```



\## 🧪 Testing \& Verification



The following commands are used to verify network connectivity and routing:



```bash

show ip interface brief

show ip route

ping \[destination-ip]

traceroute \[destination-ip]

```



The main testing objective is to verify communication between PCs located in different LAN networks.



\## 🎯 Learning Objectives



Through this project, I practiced:



\- Connecting multiple LAN networks using routers.

\- Configuring router interfaces with IPv4 addresses.

\- Implementing static routing between multiple routers.

\- Understanding next-hop addresses.

\- Troubleshooting connectivity issues.

\- Verifying routing tables and end-to-end communication.



\## 📁 Project Files



\- `router basic config.pkt` – Cisco Packet Tracer project file.



\---



\*\*Author:\*\* Khaled Hassan



\*\*Field:\*\* Computer Networking | CCNA Fundamentals

