# CSRF-Lab-03
This is [Link-Lab](https://portswigger.net/web-security/csrf/lab-token-validation-depends-on-token-being-present).
<br />

# Solve Lab-03
1- Login as wiener/peter.
<br />

![login](screenshots/1.png)
<br />

2- Intersection the request in `proxy` tab and send to `Repeater`, then try delete the csrf token --> will appear 302 status code redirection code.
<br />

![remove-csrf](screenshots/2.png)
<br />

3- After redirection.
<br />

![redirection](screenshots/3.png)
<br />

4- try to change `csrf` token, will appear message `Invaild csrf token`.
<br />

![invailed-csrf](screenshots/4.png)
<br />

5- To exploit this vulnerability to use the script, and run `python.exe -m http.server 5555` in terminal.
<br />

![http.server](screenshots/5.png)
<br />

6- OR go to `Go to exploit server`, then copy and past the html in the body section, finally solved the lab.
<br />

![exploit-server](screenshots/6.png)
<br />