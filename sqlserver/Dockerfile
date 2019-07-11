FROM mcr.microsoft.com/mssql/server:2019-CTP3.1-ubuntu

RUN apt-get install apt-transport-https

ENV TZ=Asia/Bangkok
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

RUN apt-get update
