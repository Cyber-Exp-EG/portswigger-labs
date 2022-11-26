# CSRF-Lab-06.
This is [Link-Lab](https://portswigger.net/web-security/csrf/lab-token-duplicated-in-cookie).
<br />

# Solve Lab-06.
1- login as wiener/peter, and intersection the request and check it, you will find `csrf token and session` are same.
<br />

![csrf](screenshots/1.png)
<br />

2- Try change value of `csrf session and token` with another value, for example: `test`.
<br />

![csrf](screenshots/2.png)
<br />

3- After send the request, you will find the message `302 code status redirection`.
<br />

![302](screenshots/3.png)
<br />

4- After redirection.
<br />

![redirection](screenshots/4.png)
<br />

5- Try search `hacked`, you will find new parameter `LastSearchTerm=hacked`, but we need to that add `csrf cookie while send request of search`.
<br />

![search](screenshots/5.png)
<br />

6- After send the request, look at the response.
<br />

![response](screenshots/6.png)
<br />

7- To exploit this lab and solve it, use the `scipt` html, and `Go To Exploit Victim`, then `store`, and `send to victim`.
<br />

![exploit](screenshots/7.png)
<br />

![solved](screenshots/8.png)
<br />