FROM python:3.10-alpine
RUN adduser -s /bin/sh -D getweather
USER getweather
ADD requirements.txt .
ADD geo .
RUN pip install -r requirements.txt
ENTRYPOINT [ "python3", "geo" ]