
# use official image of nginx
FROM nginx:alpine

# Remove the default Nginx config
RUN rm /etc/nginx/conf.d/default.conf

# copy your constum nginx config to container
COPY nginx.conf /etc/nginx/conf.d/

# Expose port 80 for outside world
EXPOSE 3000

# Start nginx when container starts
CMD ["nginx" "-g", "daemon off;"]