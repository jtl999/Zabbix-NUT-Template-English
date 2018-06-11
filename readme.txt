Specific template for using in PfSense with NUT package installed.
Different template needed for other file locations.

- upsc is located at /usr/local/bin/upsc
- zabbix zabbix angent configuration: to be placed under PackageServices: Zabbix Agent 3.4 / Agent / Advanced options (contents of /etc/zabbix/zabbix_agentd.conf.d/nut-ups.conf file)
- place /usr/local/sbin/nut-ups.sh at the same location

You can test working of script by running "/usr/local/sbin/nut-ups.sh ups". This will returnt a text string with the relevant UPS data.

Add the template to zabbix (import), add the template to the pfsense host and autodiscovery should do the rest.
 

