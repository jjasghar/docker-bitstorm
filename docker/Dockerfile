FROM php:7.2-fpm

RUN mkdir /app && \
    apt-get update -y && \
    apt-get install -y nginx git && \
		git clone 'https://github.com/petcap/bitstorm.git' /tmp/git/ && \
		cp /tmp/git/announce.php /app
