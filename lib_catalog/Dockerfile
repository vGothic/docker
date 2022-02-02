FROM python:3.8-slim-buster
WORKDIR /
copy requirements.txt requirements.txt
RUN pip3 install -r requirements.txt

COPY . .
#run python3 manage.py migrate
CMD python3 manage.py runserver 0.0.0.0:8000

