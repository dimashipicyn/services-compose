FROM debian:buster
RUN apt update -y && apt install -y php-fpm
RUN sed -i 's/listen = \/run\/php\/php7.3-fpm.sock/listen = 127.0.0.1:9000/' etc/php/7.3/fpm/pool.d/www.conf
CMD ["service", "php7.3-fpm", "start"]