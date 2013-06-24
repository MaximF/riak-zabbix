riak-zabbix
===========

Zabbix conf and template for Riak


1.) Install these crontabs under the riak user

* * * * /usr/sbin/riak-admin status > /var/lib/riak/riak_admin_status.tmp
* * * * /usr/sbin/riak-admin member-status > /var/lib/riak/riak_admin_member_status.tmp

2.) Deploy the attached riak.conf to /etc/zabbix/zabbix_agentd.conf.d/

3.) Import the attached zbx_export_templates.xml into Zabbix 2.x and apply to the relevant hosts and or groups

4.) Please refer to this page [0] to understand the stats you're now gathering

[0] http://docs.basho.com/riak/latest/cookbooks/Statistics-and-Monitoring/
