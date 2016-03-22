# mod_proxy_wstunnel_ssl

This module will compile for Apache 2.2.15 on RHEL6.7 or CentOS6.7.

It incorporates fixes to allow SSL Websocket proxies.

1. sudo yum install httpd-devel
2. sudo apxs -c mod_proxy_wstunnel.c
3. sudo apxs -i -a -n proxy_wstunnel mod_proxy_wstunnel.la

If you do not want to compile and just drop the module in, you can try the .so

1. cp mod_proxy_wstunnel.soi /usr/lib64/httpd/modules/
2. chmod 755 /usr/lib64/httpd/modules/mod_proxy_wstunnel.so
3. Add line to /etc/httpd/conf/httpd.conf: LoadModule proxy_wstunnel_module /usr/lib64/httpd/modules/mod_proxy_wstunnel.so
