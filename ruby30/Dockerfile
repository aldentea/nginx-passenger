FROM phusion/passenger-ruby30:latest

RUN apt-get update && \
    apt-get install libcurl4-openssl-dev && \
    passenger-install-nginx-module --auto --auto-download --prefix=/usr --languages=ruby,nodejs

EXPOSE 80

CMD ["service", "nginx", "reload"]
