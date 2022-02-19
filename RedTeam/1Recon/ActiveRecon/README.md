# Active Reconnaissance
***Active reconnaissance*** is a way of finding out information that does leave a footprint. (Think of a footprint like a digital signature, your thumb has a footprint, and so does your online activity although in a more abstract way) It involves an attempt to figure out things like the OS (Operating System) being used, any open ports, (a port being a pathway into a network basically. This is important because if you can find an open port, you can most likely find a way to get into the network) email addresses of the employees, etc.

## Scanning
#### Nmap
[Nmap](https://nmap.org/) is a free and open-source network scanner created by Gordon Lyon. Nmap is used to discover hosts and services on a computer network by sending packets and analyzing the responses. Nmap provides a number of features for probing computer networks, including host discovery and service and operating system detection. [CheatSheet](https://www.stationx.net/nmap-cheat-sheet/)
```
nmap -vv -sV -p- --script vuln 10.0.0.184
```
## Web Directory Enumeration
#### Nikto
[Nikto](https://tools.kali.org/information-gathering/nikto) is a free software command-line vulnerability scanner that scans webservers for dangerous files/CGIs, outdated server software and other problems. It performs generic and server type specific checks. It also captures and prints any cookies received.
```
nikto -H -nossl <ip.address>
nikto -id bob:bubbles -host http://10.10.195.128:1234/manager/html
```
*Nikto can be used with plugin*
```
nikto -list-plugins
nikto -Plugins+ apacheusers -H 10.10.10.10
```
#### GoBuster
[GoBuster](https://github.com/OJ/gobuster) - is a multi-threaded java application that is used to perform brute force over directories and file names on web and application servers. DirBuster attempts to find hidden directories and pages within a web application, providing users with an additional attack vector.  
```
gobusterdir -u http://10.10.195.128 -w /usr/share/wordlists/dirbuster/dirbuster-Git
```
#### DirSearch
[DirSearch](https://github.com/maurosoria/dirsearch) - is a simple command line tool designed to brute force directories and files in websites.
