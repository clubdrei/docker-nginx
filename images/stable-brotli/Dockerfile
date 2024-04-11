#
# This file is appended to the official Dockerfile of NGINX, so we can add additional build steps.
#

# Ensure that the brotli modules are actually enabled/loaded.
RUN sed -i '1i load_module /usr/lib/nginx/modules/ngx_http_brotli_filter_module.so;' /etc/nginx/nginx.conf
RUN sed -i '1i load_module /usr/lib/nginx/modules/ngx_http_brotli_static_module.so;' /etc/nginx/nginx.conf

# Add our default settings (e.g. server_tokens off)
COPY /images/stable-brotli/000-clubdrei.conf /etc/nginx/conf.d/
