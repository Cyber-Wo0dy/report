Presentation:\
Data: 30/01/2026\
Autor: David Silva

Security vulnerability: Unquoted Service Path\
Affected Component:  Total VPN

Product: Total VPN\
Version: 0.5.29.0\
Vendor: Total VPN (https://www.totalvpn.com/)

**Vulnerability Description**\
Unquoted Search Path or Element vulnerability in Total VPN. A local attacker who successfully exploited this vulnerability could gain elevated privileges by inserting an executable file in the path of the affected service. 

**Impact**\
By exploiting this vulnerability, an attacker could send a malicious .exe file to the parent directory (for example, C:\Program.exe), so Windows will interpret this path instead of the intended one, as ```C:\Program Files\Total VPN\win-service.exe```. This could allow an attacker to use the privileges of the legitimate software to perform privilege escalations, compromise data, or alter system functionality, jeopardizing the security and integrity of the environment.


**To reproduce**:
1) Note that the registered service address for the software contains spaces and no quotation marks.

![step1](img/1.png)

2) Create a malicious executable file named "Program.exe" and place it on the C:\ drive.

3) Restart the service and observe that the malicious executable file will run.