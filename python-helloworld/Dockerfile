FROM python:3.8
LABEL maintainer="Katie Gamanji"

COPY . /app

WORKDIR /app

RUN pip install --upgrade pip &&\
    pip install --trusted-host pypi.python.org -r requirements.txt

# command to run on container start
CMD [ "python", "app.py" ]