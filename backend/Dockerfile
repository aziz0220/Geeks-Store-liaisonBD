# Use the official PHP image as the base
FROM php:8.0.30-apache

RUN apt update -y
RUN apt upgrade -y

# Install the MySQLi extension
RUN docker-php-ext-install mysqli pdo pdo_mysqli


# Set the working directory
WORKDIR /var/www/html

# Copy your application code into the container
COPY . /var/www/html
