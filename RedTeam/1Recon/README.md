During the Reconnaissance phase, a malicious actor identifies a target and explores vulnerabilities and weaknesses that can be exploited within the network. As part of this process, the attacker may harvest login credentials or gather other information, such as email addresses, user IDs, physical locations, software applications and operating system details, all of which may be useful in phishing or spoofing attacks. Generally speaking, the more information the attacker is able to gather during the Reconnaissance phase, the more sophisticated and convincing the attack will be and, hence, the higher the likelihood of success.
# Passive Reconnaissance
***Passive recon*** is when you gather information about a target without directly interacting with the target. This means that you don't send any type of request to the target and therefore the target has no way of knowing that you are gathering information on them.
## OSINT
[***Open-source intelligence***](OSINT) - is the collection and analysis of data gathered from open sources (overt and publicly available sources) to produce actionable intelligence.  
* [Google Hacking DataBase](OSINT/GHDB.md)
* [TheHarvester](OSINT/TheHarvester.md) is another tool like sublist3r which is developed using Python.
* Shodan
* Maltego
* Metagoofil
* Recon-Ng
* Check Usernames
* TinEye
* Creepy
* [DNS Enumeration](OSINT/DNS.md)

## Vulnerability Database or CVE
* [ExploitDB](https://www.exploit-db.com/) - Exploit Database (ExploitDB) is an archive of exploits for the purpose of public security, and it explains what can be found on the database.
* [NVD](https://nvd.nist.gov/vuln/search) - National Vulnerability Database (NVD) is the U.S. government repository of standards based vulnerability management data represented using the Security Content Automation Protocol (SCAP).
* [CVE Mitre](https://cve.mitre.org/) - is a list of publicly disclosed cybersecurity vulnerabilities that is free to search, use, and incorporate into products and services
* ***searchsploit*** which allows you to search ExploitDB from your own machine. This is offline, and works using a downloaded version of the database, meaning that you already have all of the exploits already on your Kali Linux!

[Top](#passive-reconnaissance)

# Active Reconnaissance
***Active reconnaissance*** is a way of finding out information that does leave a footprint. (Think of a footprint like a digital signature, your thumb has a footprint, and so does your online activity although in a more abstract way) It involves an attempt to figure out things like the OS (Operating System) being used, any open ports, (a port being a pathway into a network basically. This is important because if you can find an open port, you can most likely find a way to get into the network) email addresses of the employees, etc.

## Scanning
#### Nmap
[Nmap](https://nmap.org/) is a free and open-source network scanner created by Gordon Lyon. Nmap is used to discover hosts and services on a computer network by sending packets and analyzing the responses. Nmap provides a number of features for probing computer networks, including host discovery and service and operating system detection. [CheatSheet](https://www.stationx.net/nmap-cheat-sheet/)
```
nmap -vv -sV -p- --script vuln 10.0.0.184
```
#### Nikto
[Nikto](https://tools.kali.org/information-gathering/nikto) is a free software command-line vulnerability scanner that scans webservers for dangerous files/CGIs, outdated server software and other problems. It performs generic and server type specific checks. It also captures and prints any cookies received.
```
nikto -H -nossl <ip.address>
nikto -id bob:bubbles -host http://10.10.195.128:1234/manager/html
```
***Nikto can be used with plugin***
```
nikto -list-plugins
nikto -Plugins+ apacheusers -H 10.10.10.10
```

## Web Directory Enumeration
#### GoBuster
[GoBuster](https://github.com/OJ/gobuster) - is a multi-threaded java application that is used to perform brute force over directories and file names on web and application servers. DirBuster attempts to find hidden directories and pages within a web application, providing users with an additional attack vector.  
```
  gobusterdir -u http://10.10.195.128-w/usr/share/wordlists/dirbuster/dirbuster-Git
```
#### DirSearch
[DirSearch](https://github.com/maurosoria/dirsearch) - is a simple command line tool designed to brute force directories and files in websites.

[Top](#passive-reconnaissance)
