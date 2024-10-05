# Network Enumeration with Nmap

## Description

This project demonstrates the use of Nmap (Network Mapper) for network enumeration and discovery. Nmap is a powerful open-source tool used by security professionals and network administrators to explore networks, perform security scans, and discover live hosts and services.

## Tool Used

- **Nmap** (Network Mapper)

## Environment

- Virtual Box (Kali Linux)
- Target network (lab environment)

## Basic Usage

```
nmap [Scan Type] [Options] {target specification}
```

## Common Scanning Techniques

1. **Basic Scan**
   ```
   nmap 192.168.1.1
   ```

2. **Scan a Range of IPs**
   ```
   nmap 192.168.1.1-254
   ```

3. **Scan a Subnet**
   ```
   nmap 192.168.1.0/24
   ```

4. **Aggressive Scan**
   ```
   nmap -A 192.168.1.1
   ```

5. **Port Scan**
   ```
   nmap -p 1-65535 192.168.1.1
   ```

6. **OS Detection**
   ```
   nmap -O 192.168.1.1
   ```

7. **Scan for Vulnerable Services**
   ```
   nmap --script vuln 192.168.1.1
   ```

## Example Outputs


1. Basic Scan Result
<img src="https://i.imgur.com/jnGKaKy.png" height="80%" width="80%" />
<br />
<br />
2. Port Scan Output
<img src="https://i.imgur.com/W7Q5MCc.png" height="80%" width="80%" />
No OS detected.
<br />
<br />
3. Example OS Detection Result
<img src="https://i.imgur.com/JWrR4Pn.png" height="80%" width="80%" />
This is what an OS detection looks like on a port.

4. Nmap Scan report for devices on a network
<img src="https://i.imgur.com/vpqfPFf.png" height="80%" width="80%" />
Covered Mac Adresses for safety, list of all devices on my home network. 

## Safety and Legal Considerations

- Always obtain explicit permission before scanning networks you do not own or manage.
- Be aware that aggressive scanning can be disruptive and may be detected as malicious activity.
- Use Nmap responsibly and ethically.

## Additional Resources

- [Nmap Official Documentation](https://nmap.org/book/man.html)
- [Nmap Network Scanning Book](https://nmap.org/book/)

## Disclaimer

This tool is for educational purposes only. The user assumes all responsibility for the use of this tool and must comply with all applicable local, state, and federal laws.
