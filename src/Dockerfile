# Use the lightweight nginx image
FROM nginx:alpine

# Remove the default nginx index (optional)
RUN rm -f /usr/share/nginx/html/*

# Copy our static site files into the nginx html directory
COPY index.html /usr/share/nginx/html/index.html

# (Optional) copy other static assets if you have them:
# COPY assets/ /usr/share/nginx/html/assets/

# Expose port 80 (informational; docker run -p controls actual host mapping)
EXPOSE 80

# Use the default nginx command (daemon off)
CMD ["nginx", "-g", "daemon off;"]
