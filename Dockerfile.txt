# Use the official nginx image from Docker Hub
FROM nginx:alpine

# Copy the contents of the 'src' folder to the nginx html folder
COPY ./src /usr/share/nginx/html

# Expose port 80 for HTTP
EXPOSE 80

# Start nginx server
CMD ["nginx", "-g", "daemon off;"]
