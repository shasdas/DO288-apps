# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent
EXPOSE 8080
RUN sed -i "s/Listen 80/Listen 8080/g" /etc/httpd/conf/httpd.conf
RUN chown :root /var/run/httpd /var/log/httpd &&
    chmod g=u /var/run/httpd /var/log/httpd
USER 1001
