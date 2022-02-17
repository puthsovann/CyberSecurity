
# Phishing Email

Below are typical characteristics phishing emails have in common:
* The sender email name/address will masquerade as a trusted entity (email spoofing)
* The email subject line and/or body (text) is written with a sense of urgency or uses certain keywords such as Invoice, Suspended, etc.
* The email body (HTML) is designed to match a trusting entity (such as Amazon)
* The email body (HTML) is poorly formatted or written (contrary from the previous point)
* The email body uses generic content, such as Dear Sir/Madam.
* Hyperlinks (oftentimes uses URL shortening services to hide its true origin)
* A malicious attachment posing as a legitimate document

*Additional Resources 2 Read*

[Knowbe4](https://www.knowbe4.com/phishing)
[IT Governance](https://www.itgovernance.co.uk/blog/5-ways-to-detect-a-phishing-email)
[Cheap SSL](https://cheapsslsecurity.com/blog/10-phishing-email-examples-you-need-to-see/)
[Phish Quiz](https://phishingquiz.withgoogle.com)

# Resources/Tools
## Email Header
Messageheader analyzes SMTP message headers, which help identify the root cause of delivery delays. You can detect misconfigured servers and mail-routing problems.
[GoogleApps](https://toolbox.googleapps.com/apps/messageheader/analyzeheader)
[Azure](https://mha.azurewebsites.net/)
[MailHeader Org](https://mailheader.org/)

## IP/Url Info
[IPInfo]( https://ipinfo.io/)
"With IPinfo, you can pinpoint your users’ locations, customize their experiences, prevent fraud, ensure compliance, and so much more".

[Url Scan](https://urlscan.io/)

urlscan.io is a free service to scan and analyse websites. When a URL is submitted to urlscan.io, an automated process will browse to the URL like a regular user and record the activity that this page navigation creates. This includes the domains and IPs contacted, the resources (JavaScript, CSS, etc) requested from those domains, as well as additional information about the page itself. urlscan.io will take a screenshot of the page, record the DOM content, JavaScript global variables, cookies created by the page, and a myriad of other observations. If the site is targeting the users one of the more than 400 brands tracked by urlscan.io, it will be highlighted as potentially malicious in the scan results

[Talos Reputation Center](https://talosintelligence.com/reputation)

[URL Extractor](https://www.convertcsv.com/url-extractor.htm)
The tool use for extract all url in provided header or files.

## File Reputation
[VirusTotal](https://www.virustotal.com/gui/)

[Talos File Reputation](https://talosintelligence.com/talos_file_reputation)
The Cisco Talos Intelligence Group maintains a reputation disposition on billions of files. This reputation system is fed into the AMP, FirePower, ClamAV, and Open-Source Snort product lines. The tool below allows you to do casual lookups against the Talos File Reputation system. This system limits you to one lookup at a time, and is limited to only hash matching. This lookup does not reflect the full capabilities of the Advanced Malware Protection (AMP) system.
