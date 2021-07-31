FROM tiangolo/nginx-rtmp:latest
COPY nginx.conf /etc/nginx/nginx.conf
RUN apt-get -y update \
  && apt install -y ffmpeg \
  && mkdir -p /var/www/vhosts/broadcast_streaming \
  && chmod -R o+rwx /var