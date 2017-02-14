# docker-alpine-elk

To create your own certs:

cd files

openssl req -config /etc/ssl/openssl.cnf -subj '/CN=*/' -x509 -days 3650 -batch -nodes -newkey rsa:2048 -keyout logstash-forwarder.key -out logstash-forwarder.crt
