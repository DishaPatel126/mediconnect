# Python backend Dockerfile
FROM python:3.11-slim

WORKDIR /app

COPY backend/requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY backend/ .

ENV FLASK_APP=app.py

CMD ["flask", "run", "--host=0.0.0.0"]
