FROM httpd:2.4.48
# Copy apache configuration
COPY ./httpd.conf /usr/local/apache2/conf/httpd.conf
# Copy extope configuration
COPY ./httpd_extope.conf /usr/local/apache2/conf/httpd_proxy.conf
# Expose ports
EXPOSE 80
EXPOSE 443

# Start Apache
# CMD ["/usr/sbin/httpd","-D","FOREGROUND"]
# --add-host=host.docker.internal:host-gateway
