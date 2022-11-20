FROM python:3.9

LABEL maintainer="Yegane Amirjani yeganeh.a.m7979@gmail.com"

ENV PYTHONUNBUFFERED 1

RUN python -m pip install --upgrade pip

COPY ./requirements.txt /requirements.txt
RUN pip install -r /requirements.txt

EXPOSE 18080

WORKDIR /app
COPY . /app

CMD ["python", "app.py"]
