# CSRF-Lab-08.
This is [Link-Lab](https://portswigger.net/web-security/csrf/lab-referer-validation-broken).
# Solve Lab-08.
1- 1- login as `wiener/peter`, and intersection the request and check it, you will not find `csrf token and session`, and try send the request, you will appear `302 status code redirection`. 
<br />

![1](screenshots/1.png)
<br />

2- After redirection.
<br />

![2](screenshots/2.png)
<br />

3- Testing Referer header for CSRF attacks --> remove the Referer header.
<br />

![3](screenshots/3.png)
<br />

4- Your will appear message `Invalid referer header`.
<br />

![4](screenshots/4.png)
<br />

5- Try remove value of referer header and change with another value.
<br />

![5](screenshots/5.png)
<br />

6- Try again, `Check which portion of the referrer header is the application validating`.
<br />

![6](screenshots/6.png)
<br />

7- To exploit this lab, using `html script` copy and past in body --> `Go To victim server`.
<br />

![7](screenshots/7.png)
<br />

8- Finally solved the lab.
<br />

![8](screenshots/8.png)
<br />