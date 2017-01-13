FROM nginx:stable
COPY ./config/site.conf /etc/nginx/conf.d/default.conf
COPY ./config/fastcgi_params /etc/nginx/fastcgi_params
# Debug tools
#RUN apt-get update && apt-get install -y \
#nano \
#wget \
#dialog \
#net-tools \
#curl