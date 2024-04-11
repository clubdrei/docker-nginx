# This is appended to the official Dockerfile of NGINX. It ensures that the brotli modules are actually enabled/loaded.
RUN sed -i '1i load_module /usr/lib/nginx/modules/ngx_http_brotli_filter_module.so;' /etc/nginx/nginx.conf
RUN sed -i '1i load_module /usr/lib/nginx/modules/ngx_http_brotli_static_module.so;' /etc/nginx/nginx.conf

