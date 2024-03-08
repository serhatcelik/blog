---
hide:
- navigation
---

# Port Numbers

## Table Legend

| Cell | Description |
|:---|:---|
| {++Yes++} | Described protocol is assigned by IANA for this port, and is: standardized, specified, or widely used for such. |
| {--Assigned--} | Described protocol is assigned by IANA for this port, but is not: standardized, specified, or widely used for such. |
| {==Reserved==} | Port is reserved by IANA, generally to prevent collision having its previous use removed. The port number may be available for assignment upon request to IANA. |

## Well Known Ports

| Port | Service/Protocol/Application | TCP | UDP |
|:---|:---|:---|:---|
| 0 | A system allocated (dynamic) port | {==Reserved==} | {==Reserved==} |
| 20 | FTP data transfer | {++Yes++} | {--Assigned--} |
| 21 | FTP control (command) | {++Yes++} | {--Assigned--} |
| 22 | SSH | {++Yes++} | {--Assigned--} |
| 23 | Telnet protocol | {++Yes++} | {--Assigned--} |
| 25 | SMTP | {++Yes++} | {--Assigned--} |
| 43 | WHOIS protocol | {++Yes++} | {--Assigned--} |
| 53 | DNS | {++Yes++} | {++Yes++} |
| 80 | HTTP | {++Yes++} | {++Yes++} |
| 88 | Kerberos authentication system | {++Yes++} | {++Yes++} |
| 110 | POP3 | {++Yes++} | {--Assigned--} |
| 111 | ONC-RPC/SUN-RPC | {++Yes++} | {++Yes++} |
| 137 | NetBIOS Name Service | {++Yes++} | {++Yes++} |
| 138 | NetBIOS Datagram Service | {--Assigned--} | {++Yes++} |
| 139 | NetBIOS Session Service | {++Yes++} | {--Assigned--} |
| 143 | IMAP | {++Yes++} | {--Assigned--} |
| 161 | SNMP | {--Assigned--} | {++Yes++} |
| 162 | SNMPTRAP | {++Yes++} | {++Yes++} |
| 443 | HTTPS | {++Yes++} | {++Yes++} |
| 445 | SMB | {++Yes++} | {--Assigned--} |
| 623 | IPMI Remote Management Protocol | {++Yes++} ||
| 993 | IMAPS | {++Yes++} | {--Assigned--} |
| 995 | POP3S | {++Yes++} | {++Yes++} |

## Registered Ports

| Port | Service/Protocol/Application | TCP | UDP |
|:---|:---|:---|:---|
| 1080 | SOCKS proxy | {++Yes++} | {++Yes++} |
| 1433 | MSSQL Server database management system | {++Yes++} | {++Yes++} |
| 2049 | NFS | {++Yes++} | {++Yes++} |
| 3020 | CIFS | {++Yes++} | {++Yes++} |
| 3306 | MySQL database system | {++Yes++} | {--Assigned--} |
| 3389 | RDP (Microsoft Terminal Server) | {++Yes++} | {++Yes++} |
| 5985 | WinRM-HTTP | {++Yes++} ||
| 5986 | WinRM-HTTPS | {++Yes++} ||
