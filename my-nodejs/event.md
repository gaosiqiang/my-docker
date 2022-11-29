docker run -it node:latest /bin/bash

node -v && npm -v

npm install -g npm@9.1.2 # npm升级到9.1.2

node -v && npm -v

npm install -g hexo-cli

hexo -v

---------
# npm view hexo-cli versions && \ # 查看版本
# npm install -g hexo-cli@4.1.0 && \ # 安装指定版本hexo
# npm version && \


------------

FROM centos:7

# 安装hexo

RUN yum install -y gcc gcc++ gcc-c++ && \
wget --no-check-certificate https://nodejs.org/dist/v18.12.1/node-v18.12.1.tar.gz && \
tar zxvf node-v18.12.1.tar.gz && \
cd node-v18.12.1 && \
./configure --prefix=/usr/local/node/v18.12.1 && \
make && \
make install && \

# useing
# docker build -f Dockerfile-gaosiqiang-blog -t gaosiqiang_blog:v1 .

---------------

足球进攻，有机会直接射门，没有那么复杂，要敢想敢干；

如果人太想得到一个东西的时候会锱铢必较，也就失了智，心智变的跟小孩子一样；

官场上只要自己站得住，就会有有人挺，如果不能，不仅没人挺反而有人踩；

-----------------

FROM centos:7

# 安装hexo

RUN yum install -y gcc gcc++ gcc-c++ && \
wget --no-check-certificate https://nodejs.org/dist/v18.12.1/node-v18.12.1-linux-x64.tar.gz && \
tar zxvf node-v18.12.1-linux-x64.tar.gz && \
cd node-v18.12.1-linux-x64 && \
./configure --prefix=/usr/local/node/v18.12.1 && \
make && \
make install && \

# useing
# docker build -f Dockerfile-gaosiqiang-blog -t gaosiqiang_blog:v1 .

----------------------------------

npm install 安装最新版本nodejs
---------------------
