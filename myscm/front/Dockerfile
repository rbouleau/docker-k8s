FROM nginx

RUN mkdir conf

ADD . /usr/share/nginx/html
ADD mime.conf /etc/nginx

CMD cp /conf/myscm/nginx.conf /etc/nginx/nginx.conf; service nginx restart

