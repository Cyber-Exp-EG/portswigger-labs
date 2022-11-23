# CSRF-Lab-04
This is [Link-Lab](https://portswigger.net/web-security/csrf/lab-token-not-tied-to-user-session).
<br />

# Solve Lab-04
1- login as wiener/peter.
<br />

![login-1](screenshots/1.png)
<br />

2- Try remove `csrf token` and send request, then show message `Missing Parameter 'csrf' `.
<br />

![remove-csrf](screenshots/2.png)
<br />

3- Convert request method from `post` to `get`, then show `Method Not Allowed.`.
<br />

![get-method](screenshots/3.png)
<br />

4- Try that modify on the `csrf token`, then show `Invalid CSRF Token`.
<br />

![csrf-modify](screenshots/4.png)
<br />

5- After doing the last steps, try login as `carlos/montoy`.
<br />

![login-again](screenshots/5.png)
<br />

6- Inspect in input email --> copy and past `csrf` for `carlos` and past override `csrf` for `peter`, the show `302 code status` redirection.
<br />

![redirection](screenshots/6.png)
<br />

7- After redirection.
<br />

![after](screenshots/7.png)
<br />

8- To exploit this vulnerability to use the script, and run `python3 -m http.server 5555` in terminal. 
<br />

![exploit](screenshots/8.png)
<br />

9- OR go to `Go to exploit server`, then past the `html` in the body section, then show `solved` lab.
<br />

![exploit-2](screenshots/9.png)
<br />