FROM php:cli

RUN pecl install swoole \
	&& docker-php-ext-enable swoole
	
copy index.php /var/www

EXPOSE 9501

ENTRYPOINT ["php", "/var/www/index.php", "start"]