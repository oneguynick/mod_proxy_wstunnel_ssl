# mod_proxy_wstunnel_ssl

This module will compile for Apache 2.2.15 on RHEL6.7 or CentOS6.7.

It incorporates fixes to allow SSL Websocket proxies.

1. sudo yum install httpd-devel
2. sudo apxs -c mod_proxy_wstunnel.c
3. sudo apxs -i -a -n proxy_wstunnel mod_proxy_wstunnel.la
