Presentation:\
Data: 18/03/2025\
Autor: David Silva

Security vulnerability: Broken Access Control\
Affected Component:  The “Theme Editor" page\
CVSS:4.0/AV:N/AC:L/AT:N/PR:L/UI:N/VC:H/VI:H/VA:N/SC:N/SI:N/SA:N

Product: Juzaweb CMS\
Version: 3.4.2\
Vendor: Juzaweb (https://juzaweb.com/)

Vulnerability Description\
An unprivileged user can access and modify functions related to the theme editing page.

Impact\
By exploiting this vulnerability, a malicious user with low privileges will be able to manipulate the CMS theme as an administrative user.

To reproduce:
1) Create a new user and add it to a role with all permissions disabled;

2) Log in with this user's account;

3) Access the address http://your-application.com/admin-cp/theme/editor/default ;

4) Note that the user can access and edit functions related to the theme editing:

![step4](img/1a.png)

![step5](img/2.png)

![step6](img/3.png)

![step7](img/4.png)