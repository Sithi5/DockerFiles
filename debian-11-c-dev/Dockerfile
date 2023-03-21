FROM debian:11

RUN apt-get update && \
    apt-get install -y build-essential valgrind vim git man-db && \
    apt-get install -y inetutils-ping && \ # For ft_ping 42 project
    rm -rf /var/lib/apt/lists/*

VOLUME /shared

COPY .bashrc /root/
COPY .vimrc /root/


CMD ["bash"]


# Build the container with:
# docker build -t my-image .

# to run it with a shared directory:
# docker run -it -v /path/to/host/dir:/shared my-image

