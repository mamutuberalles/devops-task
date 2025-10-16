FROM python:3.13-alpine

WORKDIR /app

COPY requirements.txt .
RUN pip install -r requirements.txt

COPY helloapp/ ./helloapp/

CMD ["gunicorn", "--bind", "0.0.0.0:8080", "-w", "2", "helloapp.app:app"]