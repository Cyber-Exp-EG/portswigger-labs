# CSRF-Lab-01
This is ![Link-Lab](https://portswigger.net/web-security/csrf/lab-no-defenses).
<br />

# Solve Lab-01
1- login as wiener/peter.
<br />

![step-1](screenshots/1.png)
<br />
2- intersection the request in `Proxy` tab and send to `Repeter`.
<br />

![step-2](screenshots/2.png)
<br />
3- Change the email the send request then appear 302 status code redirection message.
<br />

![step-3](screenshots/3.png)
<br />
4- After redirection.
<br />

![step-4](screenshots/4.png)
<br />
5- Then go to terminal in the location file `python3 -m http.server 9000`, go to the browser `127.0.0.1:9000/file_name`, go to the lab tab, wil find email changed.
<br />

![step-5](screenshots/5.png)
<br />
6- Final To solve this lab go to `Go to exploit server` in lab tab, then past the `html` in the `body` section, then press `Dilever exploit to victim`.
<br />

![step-6](screenshots/6.png)