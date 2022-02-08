FROM php:7.1-apache


RUN apt-get update && apt-get install -y \
        libpng-dev \
        software-properties-common \
        zlib1g-dev \
        libxml2-dev \
        libzip-dev \
        libonig-dev \
        zip \
        curl \
        apt-utils \
        iputils-ping \
        unzip \
    && docker-php-ext-configure gd \
    && apt install -y \
        g++ \
        libicu-dev \
        libpq-dev \
        libzip-dev \
        zip \
        zlib1g-dev \
    && docker-php-ext-install \
        intl \
        opcache \
        pdo \
        pdo_pgsql \
        pgsql \
    && docker-php-ext-install zip \
    && docker-php-source delete
