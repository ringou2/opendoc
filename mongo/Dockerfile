FROM nginx:alpine
ENV TARGET=/usr/share/nginx/html

COPY default.conf /etc/nginx/conf.d/default.conf

# Set the default command to serve the static HTML site
CMD echo -e "Docker docs are viewable at:\nhttp://0.0.0.0:4000"; exec nginx -g 'daemon off;'
#wget https://docs.mongodb.com/v4.2/manual.tar.gz


RUN wget https://docs.mongodb.com/v4.2/manual.tar.gz && \
tar -xzf manual.tar.gz -C /usr/share/nginx/ --strip-components 1 &&  