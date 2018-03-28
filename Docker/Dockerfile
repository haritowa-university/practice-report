FROM ubuntu

WORKDIR /container
ADD scalable-cyrfonts.deb /container

RUN apt-get update -qq -y

RUN apt-get install texlive-full -y
RUN apt-get install python-pygments -y

RUN rm -rf /tmp/* /var/tmp/*
RUN apt-get clean && rm -rf /var/lib/apt/lists/*
RUN rm -rf /usr/share/doc/

CMD ["dpkg", "scalable-cyrfonts.deb"]
