# CSRF-Lab-02
This is [Link-Lab](https://portswigger.net/web-security/csrf/lab-token-validation-depends-on-request-method).
<br />

# Solve Lab-02
1- login as wiener/peter.
<br />

![login](screenshots/1.png)
<br />

2- intersection the request in `proxy` tab and send to `Repeater`.
<br />

3- try delete the `csrf` token then send request, but 400 status code is a not found page.
<br />

![two](screenshots/2.png)
<br />

4- change the method `post` to `get` request then send request, will appear 302 status code is a redirection message.
<br />

![three](screenshots/3.png)
<br />

5- After redirection.
<br />

![four](screenshots/4.png)
<br />

6- try delete `csrf` token in `get` method, will appear redirection code status 302 redirection.
<br />

![five](screenshots/5.png)
<br />

7- To exploit this vulnerability to use the script, and run `python3 -m http.server 9999` in terminal.
<br />

![six](screenshots/6.png)
<br />

8- Go to browser and write in tab `127.0.0.1:9999/csrf-lab-02.html`.
<br />

![seven](screenshots/7.png)
<br />

9- Go to tab lab, will find email changed.
<br />

![eight](screenshots/8.png)
<br />

10- OR go to `Go to exploit server`, then past the `html` in the body section.
<br />

![nine](screenshots/9.png)

11- finally, congratulations your lab is solved successfully.
<br />

![ten](screenshots/10.png)