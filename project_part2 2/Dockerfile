FROM python:3.11-alpine
WORKDIR /app
COPY book_catalog/requirements.txt /app/requirements.txt
RUN pip install --no-cache-dir -r requirements.txt
COPY book_catalog /app
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "80"]


