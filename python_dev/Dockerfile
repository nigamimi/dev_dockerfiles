FROM python:3.9.1-buster

RUN apt-get update &&\ 
    apt-get upgrade 

RUN pip install poetry && \
    mkdir /projects &&\
    cd /projects && \
    poetry new project

# ユーザーを作成
# ARG UID=1020
# ARG USER=oyasai
# ARG PASSWORD="dwaofonanfwaofljngnbralenas"
# RUN useradd -m --uid ${UID} --groups sudo ${USER} \
#   && echo ${USER}:${PASSWORD} | chpasswd

# 作成したユーザーに切り替える
# ARG USER=oyasai
# ENV USER=${USER}

CMD ["/bin/bash"]