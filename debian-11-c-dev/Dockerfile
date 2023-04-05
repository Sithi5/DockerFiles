FROM debian:11

RUN apt-get update && \
    apt-get install -y vim git man-db bc procps \
    build-essential valgrind \
    python3 python3-pip python3-venv  && \
    rm -rf /var/lib/apt/lists/*

# ping for ft_ping 42 project
# traceroute for ft_traceroute 42 project

VOLUME /shared

COPY .bashrc /root/
COPY .vimrc /root/


CMD ["bash"]


# Build the container with:
# docker build -t my-image .

# to run it with a shared directory:
# docker run -it --name debian11 -v /path/to/host/dir:/shared my-image

