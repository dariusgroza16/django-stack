FROM python:latest

RUN apt-get update -y && \
    apt-get upgrade -y

WORKDIR /app

COPY requirements.txt /app/
COPY . .

RUN pip install --upgrade pip
RUN pip install -r requirements.txt

EXPOSE 8001

CMD [ "python3", "manage.py", "runserver", "0.0.0.0:8001" ]