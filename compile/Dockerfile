FROM python:3.7
ADD . /usr/app
WORKDIR /usr/app
COPY ./scrapyd.conf /etc/scrapyd/
EXPOSE 6800
RUN pip3 install -r requirements.txt
CMD scrapyd