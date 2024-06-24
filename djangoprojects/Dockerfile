FROM python:3

COPY . /src
WORKDIR /src

RUN pip install -r requirements.txt
RUN python manage.py migrate

EXPOSE 80

ENTRYPOINT ["python", "manage.py", "runserver", "0.0.0.0:80"]
