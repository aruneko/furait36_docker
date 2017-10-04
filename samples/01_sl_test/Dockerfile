FROM ubuntu:16.04
RUN sed -i -e 's%http://.*.ubuntu.com%http://ftp.jaist.ac.jp/pub/Linux%g' /etc/apt/sources.list && \
    apt update && \
    apt install -y sl && \
    apt-get clean && \
    ln -s /usr/games/sl /usr/bin/sl
