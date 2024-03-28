# Description: This file is used to create a custom nginx image that serves the index.html file from the public folder
FROM nginx:1.10.1-alpine
#Copies the index.html file to the default nginx public html folder
COPY /public/index.html /usr/share/nginx/html
COPY /public/asset.png /usr/share/nginx/html
#Exposes the port 8080
EXPOSE 8080
#Starts the nginx server
CMD ["nginx", "-g", "daemon off;"]