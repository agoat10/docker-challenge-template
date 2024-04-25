# Use the official NGINX image from the Docker registry
FROM nginx:alpine

# Remove the default nginx index page
RUN rm -rf /usr/share/nginx/html/*

# Copy the contents of the 'public' folder to the directory that nginx serves
COPY public /usr/share/nginx/html

# Expose port 80
EXPOSE 80

# Start Nginx and keep it running in the foreground
CMD ["nginx", "-g", "daemon off;"]
