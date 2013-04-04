About
========================

Using this nginx config we can check a type of users device (iPhone, iPod, iPad, Android mobile, Android tablet), detect an original size of requested image, proportionaly increase this image, cache it and return to the client.

Dependencies for nginx
========================

1. ngx_http_image_filter_module http://nginx.org/en/docs/http/ngx_http_image_filter_module.html
2. ngx_let_module https://github.com/arut/nginx-let-module
3. ngx_eval_module https://github.com/vkholodkov/nginx-eval-module

Configure nginx
========================

	./configure --with-http_image_filter_module --add-module=/path/to/ngx_let_module --add-module=/path/to/ngx_eval_module

If you will see an error message "all warnings being treated as errors" from gcc for ngx_eval_module during the "Make" process, use this solution http://stackoverflow.com/questions/5451237/nginx-0-9-6-frustrating-compile-issues-ubuntu-gcc-4-6-1.
