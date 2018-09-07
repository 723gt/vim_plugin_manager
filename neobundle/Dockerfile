FROM ubuntu:18.04  
MAINTAINER 723ch (GitHub: https://github.com/723gt/vim_plugin_manager)

WORKDIR /root
RUN apt update && apt upgrade -y && apt install -y git vim curl
RUN curl https://raw.githubusercontent.com/Shougo/neobundle.vim/master/bin/install.sh > install.sh && sh ./install.sh
COPY ./.vimrc /root/
CMD /bin/bash
