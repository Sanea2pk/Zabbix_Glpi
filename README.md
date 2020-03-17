## Zabbix integration with GLPI
These scripts automatic opening and closing GLPI tickets using API.

Source: https://github.com/janssenlima/zabbix-glpi
> **Tested and running on Ubuntu 18.04 64 bit.**
## Requirements
-**Script**: 
 - ack_zabbix_glpi.py is the script that recognizes the event in Zabbix via API.
 - tickets_zabbix_glpi.php is the script that opens and closes tickets in GLPI using the Webservices plugin.
 
- **Zabbix 4.4.1**
- **PHP 5.6**

     Include: (for both servers)
    - **php-soap**
    - **php-xmlrpc**
- **GLPI 4.9.5**
    - **Webservices Plugin** install latest from https://forge.glpi-project.org/projects/webservices/files
- **Python 2.7**
- API Zabbix development in Python, just execute in terminal -> # **pip install zabbix-api** ( on both servers: **GLPI** and **Zabbix** - if they are on different linux servers )

## Installing
Download scripts: **ack_zabbix_glpi.py** and **tickets_zabbix_glpi.php** and mvoe into zabbix directory: **_/usr/lib/zabbix/externalscripts_**.

-> # mv * zabbix * /usr/lib/zabbix/externalscripts/

-> # chmod + x /usr/lib/zabbix/externalscripts/* zabbix *


