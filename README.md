# DHCP-Starvation
DHCP starvation is an attack where a malicious user sends a large number of DHCP (Dynamic Host Configuration Protocol) requests to a DHCP server using fake MAC addresses. This causes the DHCP server to run out of IP addresses, preventing legitimate users from obtaining an IP address and connecting to the network. 

DHCP starvation is a type of denial-of-service (DoS) attack targeting the Dynamic Host Configuration Protocol (DHCP) server in a network. DHCP is responsible for dynamically assigning IP addresses and other network configuration details to devices as they join a network. In a DHCP starvation attack, an attacker floods the DHCP server with an overwhelming number of DHCP requests, each requesting an IP address, typically using spoofed MAC addresses.

The goal of this attack is to exhaust the DHCP server's pool of available IP addresses, causing legitimate devices to be unable to obtain an IP address. Without an IP address, devices cannot communicate on the network, leading to service disruptions or network downtime. In some cases, attackers may also attempt to cause additional network instability by injecting malicious DHCP responses, further complicating the situation.

In this report, we will explore the mechanics of DHCP starvation, its potential impact on network security, and various mitigation strategies to prevent or mitigate this attack.
