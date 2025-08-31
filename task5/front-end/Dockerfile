FROM nginx:latest

# paste code front
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# paste config Nginx
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# expose port 9000
EXPOSE 9000
