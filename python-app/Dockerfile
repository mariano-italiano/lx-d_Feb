FROM python:3.12-slim-bullseye

#MAINTAINER Marcin Kujawski
LABEL "Author"="Marcin Kujawski"

WORKDIR /app

COPY requirements.txt .
#COPY app.py .

RUN pip3 install --no-cache-dir -r requirements.txt

RUN adduser flaskuser

COPY --chown=flaskuser:flaskuser . . 

USER flaskuser

ENV PYTHON_ENV1="/test/path"

#CMD python3 app.py
CMD ["python3", "app.py"]
