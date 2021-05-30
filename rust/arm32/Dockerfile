FROM dockeragent-arm32:latest

RUN curl https://sh.rustup.rs -sSf | sh -s -- -y

RUN sudo apt-get update
RUN sudo apt-get install build-essential -y

ENTRYPOINT [ "./start.sh" ]
