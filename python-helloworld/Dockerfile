FROM python:3.8
LABEL maintainer="Duc Toan"

COPY ./techtrends/ /app

WORKDIR /app

RUN pip install --upgrade pip &&\
    pip install --trusted-host pypi.python.org -r requirements.txt
RUN python init_db.py

# command to run on container start
CMD [ "python", "app.py" ]