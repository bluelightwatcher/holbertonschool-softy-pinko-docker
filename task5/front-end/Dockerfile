FROM nginx:latest

# Copying files
COPY ./softy-pinko-front-end/ /var/www/html/softy-pinko-front-end
COPY ./softy-pinko-front-end.conf  /etc/nginx/conf.d/default.conf

# Setting up port
EXPOSE 9000
