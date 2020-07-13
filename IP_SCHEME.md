# IP Address Scheme
The slx ip address scheme will be optomized for systems with between (1) and (3) network switches. Systems beyond that will not be capable of conforming to the standard system and must be modified.
<br><br>
The first (3) octets of the IP address will be assigned to the project before installation. The final octet will reflect the network switch number followed by the port number.

| xxx.xxx.xxx     | x             | xx          |
|:---:            |:---:          |:---:        |
| assigned by slx | switch number | port number |

* **Switch Number = 0-2. Numbers are base 0 i.e., switch 1 is #0**
* **Port Numbers = 1-48**

* Examples
  * Device connected to Network Switch 3, Port 24 = xxx.xxx.xxx.224
  * Device connected to Network Switch 2, Port 16 = xxx.xxx.xxx.116

* Network switch ip addresses
  * Switch 1 (0) = xxx.xxx.xxx.99
  * Switch 2 (1) = xxx.xxx.xxx.199
  * Switch 3 (2) = xxx.xxx.xxx.254
* Routers
  * xxx.xxx.xxx.253 (If 1 router for the system)
  * xxx.xxx.xxx.198 (If 2nd router for the system)
  * xxx.xxx.xxx.98 (If 3rd router for the system)
* DHCP Ranges
  * 49-97
  * 149-197
  * 249-252
  
**Why?**
Because!<br>
This method allows network layout information right in the scheme. It also means that systems aren't tied to a "device range" scheme that leaves gaping holes of addresses unused. Most of the devices we use are wired, meaning we can physically tie them to a specific port on a network switch. Wireless devices can be spread among the open ranges between switch gaps.<br><br>
You may notice that addresses 49-52 aren't accounted for, well that's because those PORTS should be used for uplink, not access devices. These ports would house router connections, or switch uplinks.

# Get An Octet Assigned
* email slx@slintegrated.com with the subject line "ip scheme please" with details about your project in the body.
