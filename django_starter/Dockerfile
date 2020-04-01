FROM python:3.7-alpine

RUN mkdir /code
WORKDIR /code
ADD requirements.txt /code
RUN pip3 install --no-cache-dir  -r requirements.txt

ADD . /code/

EXPOSE 8000

CMD ["python3", "manage.py", "runserver", "0.0.0.0:8000"]

