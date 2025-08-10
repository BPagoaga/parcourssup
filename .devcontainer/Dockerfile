FROM php:8.2-cli

# Installer dépendances PHP requises par Symfony et PostgreSQL
RUN apt-get update && apt-get install -y \
    git \
    unzip \
    curl \
    neovim \
    libicu-dev \
    libzip-dev \
    libpq-dev \
    zip \
    && docker-php-ext-install intl zip pdo pdo_pgsql \
    && rm -rf /var/lib/apt/lists/*

# Installer Composer
RUN curl -sS https://getcomposer.org/installer \
    | php -- --install-dir=/usr/local/bin --filename=composer

# Installer Symfony CLI
RUN curl -sS https://get.symfony.com/cli/installer | bash \
    && mv /root/.symfony*/bin/symfony /usr/local/bin/symfony

WORKDIR /workspace
