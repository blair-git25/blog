# Week 6
___
## Learning Outcome 3

**_1.  Install and configure a firewall to allow a whitelist of ‘safe’ IP addresses.  Include in your blog a description of your configuration including screenshots._**

#### 1. Installation

The firewall we will be installing is called Uncomplicated Firewall, or UFW for short. It's a user-friendly command line tool for managing Linux's netfilter firewall and simplifies the complex iptables rules for allowing/blocking traffic. 

To install UFW we will run this script:
```
sudo apt install ufw
```
This installs the UFW software packages. It is disabled by default, and before we enable it we need to configure some basic rules.

#### 2. Configuration

To start of with, we will set the default policies. These default rules are already setup after installation, but we will be explicit in doing them for best practises - don't assume it's configured. These are restrictive as it denies all incoming traffic, but ensures the host can still receive updates at a base level.

```
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

Now we can add our 'safe' IP's to the allow list:

```
sudo ufw allow from 192.168.1.100
```
This allows the host on IP 192.168.1.100 access to all ports on our machine running UFW.
To increase security we can lock down access even further by only allowing certain ports to be communicated through:
```
sudo ufw allow from 192.168.1.99 to any port 22
```
This will only allow access by 192.168.1.99 on port 22, the SSH port.

#### Enable firewall

After adding all the necessary IP rules we can go ahead and enable the firewall:
```
sudo ufw enable
```
UFW will warn you that enabling it may disrupt existing connections. Type y and press Enter to proceed. 
The firewall will now be active and will automatically launch on boot. 

To check the rules we've implemented at any time we can run:
```
sudo ufw status verbose
```
This will display a clear list of allowed IPs and policies.