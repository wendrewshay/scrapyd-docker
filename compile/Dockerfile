FROM python:3.7

ENV LANG en_US.utf8

ADD . /usr/app
WORKDIR /usr/app

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

COPY ./scrapyd.conf /etc/scrapyd/
EXPOSE 6800
RUN pip3 install -r requirements.txt && pip3 install git+https://github.com/scrapy/scrapyd-client
CMD scrapyd
