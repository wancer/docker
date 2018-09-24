FROM php:fpm

RUN apt-get update && apt-get install -y \
	libfreetype6-dev \
	libjpeg62-turbo-dev \
	libpng-dev \
        &&  rm -rf /var/lib/apt/lists/*

CMD ["php-fpm"]
