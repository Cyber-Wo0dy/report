Presentation:\
Data: 18/03/2025\
Autor: David Silva

Security vulnerability: Broken Access Control\
Affected Component:  The "Add New Themes" page\
CVSS:4.0/AV:N/AC:L/AT:N/PR:L/UI:N/VC:N/VI:L/VA:N/SC:N/SI:N/SA:N

Product: Juzaweb CMS\
Version: 3.4.2\
Vendor: Juzaweb (https://juzaweb.com/)

Vulnerability Description\
An unprivileged user can upload new themes.

Impact\
By exploiting this vulnerability, a user with few privileges can import arbitrary themes into the CMS.

To reproduce:
1) Create a new user and add it to a role with all permissions disabled;

2) Log in with that user's account;

3) Go to http://your-application.com/admin-cp/theme/install ;

4) Note that the user can upload new themes to the CMS:

![step4](img/1h.png)

![step5](img/2h.png)