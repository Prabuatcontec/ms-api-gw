FROM nginx

# Install apache2-utils for basic auth
RUN apt-get update \
 && apt-get install -y --no-install-recommends \
      apache2-utils \
 && rm -rf /var/lib/apt/lists/*

ADD /nginx/html /usr/share/nginx/html
ADD /nginx/html /etc/nginx/html
ADD /nginx/nginx_root.conf /etc/nginx/nginx.conf
ADD /nginx/sites-enabled /etc/nginx/conf.d/


EXPOSE 80 
