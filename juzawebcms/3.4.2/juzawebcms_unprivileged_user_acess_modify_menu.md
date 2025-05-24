Presentation:\
Data: 18/03/2025\
Autor: David Silva

Security vulnerability: Broken Access Control\
Affected Component:  The "Menu" page\
CVSS:4.0/AV:N/AC:L/AT:N/PR:L/UI:N/VC:N/VI:L/VA:N/SC:N/SI:N/SA:N

Product: Juzaweb CMS\
Version: 3.4.2\
Vendor: Juzaweb (https://juzaweb.com/)

Vulnerability Description\
A non-privileged user can list and modify the CMS menus.

Impact\
By exploiting this vulnerability, a user with low privileges can make arbitrary changes to the CMS menus.

To reproduce:
1) Create a new user and add it to a role with all permissions disabled;

2) Log in with this user's account;

3) Access the address http://your-application.com/admin-cp/menus ;

4) Note that the user can access and modify the functions related to the CMS menu:

![step4](img/1j.png)

