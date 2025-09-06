# Ports

## Overview
Ports can range from 1 to 65,535; below are 3 categories of ports
- **Well-Known Ports:** 1 to 1,023 are desitnation ports associated with common network applications
- **Registered Ports:** 1,024 to 49,151 can be ussed as either source or destination ports; can be used by organizations to register specific applications such as IM
- **Private Ports:** 49,152 to 65,535 are often used as source ports; can be used by any application

## Well-Known Ports
| Port Number | Transport | Application Protocol                             |
|-------------|-----------|--------------------------------------------------|
| 20          | TCP       | File Transfer Protocol (FTP) - Data              |
| 21          | TCP       | FTP - Control                                    |
| 22          | TCP       | Secure Shell (SSH)                               |
| 23          | TCP       | Telnet                                           |
| 25          | TCP       | Simple Mail Transfer Protocol (SMTP)             |
| 53          | UDP, TCP  | Domain Name Service (DNS)                        |
| 67          | UDP       | Dynamic Host Configuration Protocol (DHCP) - Server |
| 68          | UDP       | DHCP - Client                                    |
| 69          | UDP       | Trivial File Transfer Protocol (TFTP)            |
| 80          | TCP       | Hypertext Transfer Protocol (HTTP)               |
| 110         | TCP       | Post Office Protocol version 3 (POP3)            |
| 143         | TCP       | Internet Message Access Protocol (IMAP)          |
| 161         | UDP       | Simple Network Management Protocol (SNMP)        |
| 443         | TCP       | Hypertext Transfer Protocol Secure (HTTPS)       |

## Troubleshooting
Command: "netstat" to view all open connections
