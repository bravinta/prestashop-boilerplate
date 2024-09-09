FROM prestashop/prestashop:latest

# Cambia el UID del usuario www-data
RUN usermod -u 1000 www-data

# Cambia el grupo del usuario www-data si es necesario
RUN groupmod -g 1000 www-data

# Cambia la propiedad del directorio /var/www y subdirectorios
RUN chown -R www-data:www-data /var/www

# Configura los permisos adecuados
RUN chmod -R 755 /var/www/var/cache
