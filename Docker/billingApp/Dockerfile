FROM nginx:stable-alphine

#use a volume is more efficient and speed that filesystem
VOLUME /tmp

#Install web app on nginx server
RUN rm -rf /usr/share/nginx/html/*
COPY nginx.conf /etc/nginx/nginx.conf
COPY dist/billingApp /usr/share/nginx/html
COPY mime.types /etc/nginx/mime.types



