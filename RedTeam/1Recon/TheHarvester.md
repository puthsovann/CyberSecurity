# The Harvester
This tool can be used by penetration testers for gathering information of emails, sub-domains, hosts, employee names, open ports, and banners from different public sources like search engines, PGP key servers, and SHODAN computer database. This tool can be used in passive reconnaissance and by anyone who needs to know what an attacker can see about the organization.

## How to install theHarvester
```
sudo apt-get theharvester
```
```
git clone https://github.com/laramies/theHarvester.git
cd theHarvester
sudo python ./theHarvester.py
```
```
Usage: theharvester options

       -d: Domain to search or company name
       -b: data source: baidu, bing, bingapi, dogpile, google, googleCSE,
                        googleplus, google-profiles, linkedin, pgp, twitter, vhost,
                        virustotal, threatcrowd, crtsh, netcraft, yahoo, all

       -s: start in result number X (default: 0)
       -v: verify host name via dns resolution and search for virtual hosts
       -f: save the results into an HTML and XML file (both)
       -n: perform a DNS reverse query on all ranges discovered
       -c: perform a DNS brute force for the domain name
       -t: perform a DNS TLD expansion discovery
       -e: use this DNS server
       -p: port scan the detected hosts and check for Takeovers (80, 443, 22, 21, 8080)
       -l: limit the number of results to work with(bing goes from 50 to 50 results,
            google 100 to 100, and pgp doesn't use this option)
       -h: use SHODAN database to query discovered hosts

Examples:
        theharvester -d microsoft.com -l 500 -b google -h myresults.html
        theharvester -d microsoft.com -b pgp
        theharvester -d microsoft -l 200 -b linkedin
        theharvester -d apple.com -b googleCSE -l 500 -s 300
```
## Example
```
theharvester -d kali.org -l 200 -b bing
```
