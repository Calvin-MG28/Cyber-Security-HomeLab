# Cyber-Security-HomeLab

In this lab, I successfully exploited a known vulnerability in the vsftpd 2.3.4 FTP service on a Metasploitable2 virtual machine using Metasploit Framework. This vulnerability (CVE-2011-2523) allows an attacker to trigger a malicious backdoor embedded in the vsftpd binary, leading to a remote root shell on the target system.

I set up a full home lab environment using VirtualBox, configuring both Kali Linux as the attacker machine and Metasploitable2 as the intentionally vulnerable target. After establishing connectivity between the VMs via host-only networking, I performed initial reconnaissance using nmap to identify exposed services.

Upon confirming the FTP service and version, I launched the exploit/unix/ftp/vsftpd_234_backdoor module in Metasploit, which successfully opened a root shell on the target. Post-exploitation steps included system enumeration and reviewing the /etc/passwd file to identify local user accounts and assess further attack vectors.

This lab demonstrates my ability to:

Set up and configure virtual environments for ethical hacking

Conduct network scanning and service enumeration

Use Metasploit for real-world exploit execution

Perform basic post-exploitation enumeration and analysis
