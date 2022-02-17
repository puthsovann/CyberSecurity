### DNS Enumeration
***DNS enumeration*** is the process of locating all the DNS servers and their corresponding records for an organization. DNS enumeration will yield usernames, computer names, and IP addresses of potential target system
### Checking for RDNS.
#### AMASS
	amass enum -d http://domain.com

#### FIERCE
	fierce --domain jtrustroyal.com

#### SUBLIST3R
	sublist3r.py -d cyper.org

#### DNSTWISt -- check for misspell domain
	dnstwist -r domain.com #is to check for register
	dnstwist domain.com #check for available domain

#### SPIDERFOOT
	spiderfoot -l 0.0.0.0:7060 #to access spiderfoot to scan
