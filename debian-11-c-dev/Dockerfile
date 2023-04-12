FROM debian:11

RUN apt-get update && \
    apt-get install -y vim git man-db bc procps \
    build-essential valgrind \
    python3 python3-pip python3-venv && \
    rm -rf /var/lib/apt/lists/*

VOLUME /shared

COPY .bashrc /root/
COPY .vimrc /root/


# Build the container with:
# docker build -t debian11 .

# to run it with a shared directory:
# docker run -it --name debian11 -v /path/to/host/dir:/shared my-image

