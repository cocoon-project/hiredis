FROM debian:jessie


RUN echo "==> install dependencies" \
 && apt-get update \
 && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
    dialog apt-utils\
    git make build-essential \
    cmake swig check rsync gawk libpcap-dev libedit-dev libpcre3-dev \
 && rm -rf /var/lib/apt/lists/*


 RUN echo "==> install hiredis"  \
  && cd tmp \
  && git config --global http.sslVerify false \
  && git clone https://github.com/cocoon-project/hiredis.git



#  cd hiredis \
#  && mkdir -p make \
#  && cd make \
#  && cmake .. \
#  && make \
#  && make install

  CMD "bash"
