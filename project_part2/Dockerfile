# Dockerfile for book_catalog microservice

FROM python:3.12-bookworm

WORKDIR /app

COPY book_catalog/requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY /book_catalog/ .

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]