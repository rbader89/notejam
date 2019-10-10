FROM python:2.7

WORKDIR /usr/src/app

COPY ./requirements.txt ./

RUN pip install -r requirements.txt

COPY . .

WORKDIR /usr/src/app/notejam

RUN ./manage.py syncdb --noinput
RUN ./manage.py migrate

CMD ["./manage.py", "runserver"]