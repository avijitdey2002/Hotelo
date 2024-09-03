#Use an official Nginx image as a base
FROM nginx:alpine

#Set the working directory to /usr/share/nginx/html
WORKDIR /usr/share/nginx/html

#Remove default Nginx static assets
RUN rm -rf ./*

#Copy the static website files from your host to the container
COPY . .

#Expose port 80 to the outside world
EXPOSE 80

#Start Nginx when the container launches
CMD ["nginx", "-g", "daemon off;"]