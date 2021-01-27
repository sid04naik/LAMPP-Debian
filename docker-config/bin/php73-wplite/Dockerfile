FROM php:7.3-apache 
RUN apt-get update -y 
RUN apt-get install libpng-dev -y
RUN apt-get install libxml2-dev -y
RUN docker-php-ext-install mysqli
RUN docker-php-ext-enable mysqli
#RUN docker-php-ext-install pdo pdo_mysql bcmath gd zip
#RUN docker-php-ext-enable pdo pdo_mysql bcmath gd zip
RUN a2enmod rewrite md
RUN /etc/init.d/apache2 restart