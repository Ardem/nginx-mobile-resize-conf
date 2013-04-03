About
========================

Using this nginx config we can check a type of users device (iPhone, iPod, iPad, Android mobile, Android tablet), proportionaly increase the size of requested image and cache it.

Dependencies for nginx
========================

1. Nginx-let-module https://github.com/arut/nginx-let-module
2. ngx_http_image_filter_module http://nginx.org/en/docs/http/ngx_http_image_filter_module.html

Configure nginx
========================

	./configure --with-http_image_filter_module --add-module=/path/to/nginx-let-module
