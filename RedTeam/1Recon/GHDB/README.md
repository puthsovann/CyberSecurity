***The Google Hacking Database (GHDB)*** The GHDB is an index of search queries (we call them dorks) used to find publicly available information, intended for pentesters and security researchers. [Exploit DB](https://www.exploit-db.com/google-hacking-database)

```
(“Index Of” | “[To Parent Directory]”) AND “*financ*” inbody:xlsx site:somebank.com
```
### Some operators cheatsheet
Operators | Description & Example
------------ | -------------
inurl: | Value is contained somewhere in the url.  ```preventing ransomware ​inurl:fbi​```
site: | Only search within this website’s given domain. ```windows xp end of life ​site:microsoft.com```
filetype: | Search only for files, not webpages. ```nasa moon landing ​filetype:JPG```
allinurl: | Search all of the following words in the url. ```allinurl: ”blog wordpress”​ information security```
intext: | Search the body of the webpage for specific text. ``` patient record ​intext:"index of /htdocs"```
related: | Find website results that are related to your search term. ```related:sans.org ```
info: | Find supplemental information Google may have on this page.(useful for finding cached pages) ```info:www.usgs.gov```
link: | Find other pages indexed by Google that reference this link. ```link:http://www.somecompany.com/supersecretfile.doc```
“quote” | Find an exact phrase (though results may include related words). ```“Malware Hunting”```
+word | Show results with this word exactly. Do not include similar words. ```Malware +Hunter```
­word/query | Do not include this word in search results or queries. ```​Advanced Malware Hunting ­beginner ­introduction ­site:microsoft.com```
“word * word” | Wildcard. Search for anything between these two words, but include both. ```“Next * Firewalls with *”```
OR | Return results for either item. The pipe character can be used in place. ```“locky OR ransomware”```
AND (or &) | Return results with both items. Ampersand character can be used in place. ```​“cissp AND certification”​  “cissp & certification”```
[#]...[#] or numrange: | Within a range numbers ```plasma television $1000...1500```
