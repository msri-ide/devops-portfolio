#Using the Base image as NGINX
FROM nginx:latest

#Copying the index.html & style.css from local to the NGINX library
COPY index.html /usr/share/nginx/html/

COPY style.css /usr/share/nginx/html/

#Mapping and Exposing the PORT

EXPOSE 80
