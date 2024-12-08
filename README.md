# DHCP-Starvation
DHCP starvation is an attack where a malicious user sends a large number of DHCP (Dynamic Host Configuration Protocol) requests to a DHCP server using fake MAC addresses. This causes the DHCP server to run out of IP addresses, preventing legitimate users from obtaining an IP address and connecting to the network. 

DHCP starvation is a type of denial-of-service (DoS) attack targeting the Dynamic Host Configuration Protocol (DHCP) server in a network. DHCP is responsible for dynamically assigning IP addresses and other network configuration details to devices as they join a network. In a DHCP starvation attack, an attacker floods the DHCP server with an overwhelming number of DHCP requests, each requesting an IP address, typically using spoofed MAC addresses.

The goal of this attack is to exhaust the DHCP server's pool of available IP addresses, causing legitimate devices to be unable to obtain an IP address. Without an IP address, devices cannot communicate on the network, leading to service disruptions or network downtime. In some cases, attackers may also attempt to cause additional network instability by injecting malicious DHCP responses, further complicating the situation.

In this report, we will explore the mechanics of DHCP starvation, its potential impact on network security, and various mitigation strategies to prevent or mitigate this attack, and how to perform such attacks....... 

FOR EDUCATIONAL PURPOSES #ONLY

Overview of DHCP Starvation Attack

A DHCP Starvation Attack is a type of denial-of-service (DoS) attack that targets the Dynamic Host Configuration Protocol (DHCP) server within a network. DHCP is responsible for automatically assigning IP addresses and other network configuration details (like the gateway and DNS) to devices as they join the network. This process allows devices to communicate with each other on the network without manual configuration.

In a DHCP starvation attack, a malicious attacker floods the DHCP server with an overwhelming number of DHCP requests. These requests are often sent using spoofed or fake MAC addresses to impersonate multiple devices. As a result, the DHCP server is forced to allocate IP addresses from its pool to these fake requests, quickly depleting the available IP address range.

When the DHCP server runs out of available IP addresses, legitimate devices attempting to join the network cannot obtain an IP address. This leads to network disruptions where authorized users are unable to communicate, causing service outages and downtime.

Additionally, an attacker may not only exhaust the DHCP server's IP address pool but could also inject malicious DHCP responses, further destabilizing the network and potentially redirecting traffic or causing additional damage.

This attack demonstrates a serious vulnerability in the network infrastructure, particularly in environments that rely heavily on DHCP for dynamic address allocation. If left unmitigated, DHCP starvation can significantly degrade a network’s performance, making it a critical threat to network availability and security.

Tools Typically Used for DHCP Starvation Attacks

DHCPig: A popular tool for conducting DHCP starvation attacks by sending a large number of DHCP requests.

Metasploit Framework: Can be used to exploit DHCP vulnerabilities in a network.

Custom Scripts: Attackers often write their own scripts in Python or Bash to automate the DHCP request flooding process.


Potential Impacts of DHCP Starvation

1. Service Outages: Devices fail to obtain IP addresses and cannot access the network, causing downtime.


2. Network Instability: The DHCP server may become overwhelmed, leading to slow or unreliable network services.


3. Loss of Availability: Legitimate users and devices may lose access to critical network resources.
