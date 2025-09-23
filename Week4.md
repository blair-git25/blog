# Week 4
___
## Learning Outcome 2

#### Contents
1. [Blog](#1-blog)
2. [Group Activity](#2-group-activity)



___
### 1. Blog

**_You have been asked by a user to explain to them about the use of a Firewall to protect their personal PC. Write approx. 250 words describing the features of  a commonly used software based Firewall.  Include a brief description of how they might configure the Firewall to add or remove allowed programs or ports._**

#### Firewalls

A software Firewall  is a program installed on a personal PC that monitors and controls incoming/outgoing network traffic.  

A commonly used software Firewall is Windows Defender Firewall. This Firewall helps safeguard the Windows PC by filtering network traffic and blocking unauthorized access. It reduces the risk of network security threats by restricting or allowing traffic based on various properties such as IP addresses, ports, or program paths.

##### Windows Firewall features 

- Traffic Filtering - inspects all traffic and allows/blocks based on predefined rules
- Inbound/Outbound rules - can create rules for specific inbound or outbound connections 
- Application control - can block or allow network communication for specific applications and services
- Profile-Based settings: Can configure different firewall settings for various network types (Private (home), Domain (work) and Public (college))
- Port and Protocol filtering - rules can be set to allow or block access based on specific port numbers and network protocols.
- Stateful inspection - keeps track of active network connections, allowing it to make informed decisions about which packets to filter

##### Using Windows Defender Firewall - Allowing a port

1. Navigate to Control Panel>System and Security> Windows Firewall.
2. Select Advanced settings and highlight Inbound Rules in the left pane.
3. Right click Inbound Rules and select New Rule.
4. Add the port you need to open and click Next.
5. Add the protocol (TCP or UDP) and the port number into the next window and click Next.
6. Select Allow the connection in the next window and hit Next.
7. Select the network type as you see fit and click Next.
8. Name the rule something meaningful and click Finish. 


### 2. Group Activity

**_In groups investigate the features and operation of both hardware based and software based firewalls. Select an example of each type of Firewall that you would recommend for a small company, justifying your choices._**

#### Hardware firewalls

Operate as a physical device, protecting entire networks of devices, between the local network and public internet.

Features include:
- Stateless/Stateful inspection 
- Packet filtering 
- IP address filtering 
- Port & Protocol filtering 
- Network Address Translation (NAT) 
- VPN gateway 
- Intrusion Detection/Prevention (IDS/IPS) 
- Deep Packet Inspection (DPI)
- Application control
- Content filtering

Small Company choice = *Cisco Firepower 1120*
Reason: Good performance and not too expensive or overkill. Has 8x RJ45 and 4x SFP allowing for plenty of connections and future growth. It's IPS throughput is 2.6 Gbps, allowing for fast and secure traffic. Can also run the latest Cisco Threat Defense (FTD) or Cisco ASA software.


#### Software Firewalls

Operates as an installed program protecting a single machine.

Features include:
- Stateless/Stateful Inspection
- Application control 
- IP & Port filtering
- Host Intrusion Prevention (HIPS)
- Process monitoring
- Web/Content filtering
- Boot-time protection
 
Small Company choice - *Trend Micro*
Trend Micro has a long track record of being an effective protector with good support. Its an all-in-on suite, so contains not just a firewall, but options like email filtering, cloud protection and anti-ransonware. It's also easy to manage.

 

 






