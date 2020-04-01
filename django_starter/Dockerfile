FROM ubuntu:latest

RUN apt update
RUN apt install python3-pip -y
RUN mkdir /code
WORKDIR /code
ADD requirements.txt /code
RUN pip3 install  -r requirements.txt

ADD . /code/

EXPOSE 8000

CMD ["python3", "manage.py", "runserver", "0.0.0.0:8000"]

