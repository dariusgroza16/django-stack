FROM python

RUN apt update && \
    apt upgrade && \
    pip3 install django

WORKDIR /site

COPY . .

CMD [ "python3", "" ]