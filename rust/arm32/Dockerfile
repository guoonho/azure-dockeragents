FROM dockeragent-arm32:latest

RUN curl https://sh.rustup.rs -sSf | sh -s -- -y

RUN apt-get update
RUN apt-get install \
    build-essential \
    libssl-dev \
    pkg-config \
    -y

ENTRYPOINT [ "./start.sh" ]
