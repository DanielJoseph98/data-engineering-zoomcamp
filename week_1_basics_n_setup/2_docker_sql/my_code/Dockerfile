# docker build -t test:pandas .
# docker run -it test:pandas 2021-01-23
# job finished successfully for day = 2021-01-23
FROM python:3.9.1

RUN apt-get install wget
RUN pip install pandas sqlalchemy psycopg2

WORKDIR /app
COPY ingest_data.py ingest_data.py

ENTRYPOINT [ "python", "ingest_data.py"]
