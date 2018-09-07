FROM ubuntu:18.04  
MAINTAINER 723ch (GitHub: https://github.com/723gt/vim_plugin_manager)

WORKDIR /root
RUN apt updata && apt upgrade -y && apt install -y git vim curl
RUN curl https://raw.githubusercontent.com/Shougo/dein.vim/master/bin/installer.sh > installer.sh && sh ./installer.sh  ~/.vim/bundle 
COPY ./.vimrc /root/
CMD /bin/bash
