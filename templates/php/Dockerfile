FROM php:latest

# Instalar dependencias necesarias para Symfony
RUN apt-get update && apt-get install -y unzip git curl libzip-dev \
    && docker-php-ext-install zip pdo pdo_mysql

# Configurar el directorio de trabajo dentro del contenedor
WORKDIR /var/www/html

# Copiar los archivos del proyecto
COPY . .

# Exponer el puerto por defecto de Symfony
EXPOSE 8000

# Comando por defecto para iniciar el servidor Symfony
CMD ["php", "-S", "0.0.0.0:8000", "-t", "public"]