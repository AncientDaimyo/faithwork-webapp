# Use the official NGINX image
FROM nginx:latest
# Remove default NGINX configuration
RUN rm /etc/nginx/conf.d/default.conf
# Copy your custom NGINX configuration
COPY ./host/faithwork-api/nginx.conf /etc/nginx/conf.d/