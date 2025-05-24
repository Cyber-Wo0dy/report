Presentation:\
Data: 18/03/2025\
Autor: David Silva

Security vulnerability: Broken Access Control\
Affected Component:  The “General Setting" page\
CVSS:4.0/AV:N/AC:L/AT:N/PR:L/UI:N/VC:L/VI:H/VA:N/SC:N/SI:N/SA:N

Product: Juzaweb CMS\
Version: 3.4.2\
Vendor: Juzaweb (https://juzaweb.com/)

Vulnerability Description\
A non-privileged user can view and modify CMS configuration information.

Impact\
By exploiting this vulnerability, a user with low privileges can view information related to the CMS, as well as make arbitrary changes to it.

To reproduce:
1) Create a new user and add it to a role with all permissions disabled;

2) Log in with this user's account;

3) Access the address http://your-application.com/admin-cp/setting/system/general ;

4) Note that the user can view and edit fields related to the general CMS settings:

![step4](img/1e.png)

![step5](img/2e.png)
