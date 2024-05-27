FROM ubuntu

# Install Nginx
RUN apt-get update && apt-get install -y nginx

# Expose the Nginx port
EXPOSE 80

# Start Nginx
CMD ["nginx", "-g", "daemon off;"]