FROM python:3.8
LABEL maintainer="Tran Hoan"

COPY ./techtrends /app
WORKDIR /app

EXPOSE 3111

RUN pip install -r requirements.txt

RUN python init_db.py

# command to run on container start
CMD [ "python", "app.py" ]
