#Arquivo api/Dockerfile
FROM python:3.9-slim

WORKDIR /app

USER root
RUN apt-get update && apt-get install -y libpq-dev gcc

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

CMD ["python", "app.py"]
