# sqlmap
*sqlmap* is an open source penetration testing tool that automates the process of detecting and exploiting SQL injection flaws and taking over of database servers. It comes with a powerful detection engine, many niche features for the ultimate penetration tester and a broad range of switches lasting from database fingerprinting, over data fetching from the database, to accessing the underlying file system and executing commands on the operating system via out-of-band connections. [More](https://github.com/sqlmapproject/sqlmap)
```
sqlmap -r request.txt --dbms=mysql --dump sqlmap -r request.txt -p username

sqlmap -u http://domain.name --form

sqlmap --dbms=SQLite -r Burp --tamper=cspace2comment --level=3 -- dump-all
```
> testing
> testin1
