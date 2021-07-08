FROM dockeragent-arm32:latest

RUN apt-get update
RUN apt-get install ruby-full build-essential zlib1g-dev
RUN echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
RUN echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
RUN echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
RUN gem install jekyll bundler

ENTRYPOINT [ "./start.sh" ]
