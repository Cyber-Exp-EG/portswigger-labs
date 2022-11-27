# CSRF-Lab-07.
This is [Link-Lab](https://portswigger.net/web-security/csrf/lab-referer-validation-depends-on-header-being-present).
# Solve Lab-07.
1- login as `wiener/peter`, and intersection the request and check it, you will not find `csrf token and session`.
<br />

![1](screenshots/1.png)
<br />

2- Try send the request, you will appear `302 status code redirection`.
<br />

![2](screenshots/2.png)
<br />

3- After redirection.
<br />

![3](screenshots/3.png)
<br />

4- Testing Referer header for CSRF attacks --> `Remove the Referer header`.
<br />

![4](screenshots/4.png)
<br />

5- Try send the request after remove the `reserer header`, you will appear `302 status code redirection`.
<br />

![5](screenshots/5.png)
<br />

6- After redirection.
<br />

![6](screenshots/6.png)
<br />

7- To exploit this lab, using `html script` copy and past in `body --> Go To victim server`.
<br />

![7](screenshots/7.png)
<br />

8- Finally solved the lab.
<br />

![8](screenshots/8.png)
<br />