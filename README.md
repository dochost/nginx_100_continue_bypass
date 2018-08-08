**Nginx Bypass HTTP 100 Continue reponse**

This patch will enable a configuration trigger to remove the HTTP 100 Continue response code and directly stream the multi part post to your upstream server

**Installation**

from your NGINX source folder run
patch p1 < /path/to/nginx_100_continue_bypass/nginx_100_continue_bypass.patch

Tested on NGINX 1.15.2

**Usage**

To enable this feature simple add into your server directive

proxy_100_continue on;
