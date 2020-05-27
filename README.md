# IP Address Scheme
The slx ip address scheme will be optomized for systems with between (1) and (3) network switches. Systems beyond that will not be capable of conforming to the standard system and myst be modified.
<br><br>
The first (3) octets of the IP address will be assigned to the project before installation. The final octet will reflect the network switch number followed by the port number.



| xxx.xxx.xxx     | x             | xx          |
|:---:            |:---:          |:---:        |
| assigned by slx | switch number | port number |

<br>

**Switch Number = 0-2. Numbers are base 0 i.e., switch 1 is #0**

<br><br>

**Port Numbers = 1-48**

<br><br>

**Examples**

<br>
Device connected to Network Switch 3, Port 24 = xxx.xxx.xxx.224
<br>
Device connected to Network Switch 2, Port 16 = xxx.xxx.xxx.116
