FROM ubuntu

WORKDIR /container
ADD scalable-cyrfonts.deb /container

RUN apt-get update -qq -y
RUN apt-get install texlive-full -y

CMD ["dpkg", "scalable-cyrfonts.deb"]
