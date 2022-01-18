FROM staticfloat/nginx-certbot:latest

ARG HOME=/etc/nginx
ENV	TZ=Europe/Kiev

WORKDIR $HOME

COPY ./docker/prod/certbot.conf $HOME/user.conf.d/nginx_template.conf
COPY ./docker/prod/proxy.conf $HOME/user.conf.d/proxy.conf
COPY ./docker/prod/nginx.conf $HOME
