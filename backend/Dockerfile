FROM python:3.9-slim
WORKDIR /app
COPY . .
RUN pip install --upgrade pip
RUN pip install -r requirements.txt --no-cache-dir
CMD ["gunicorn", "--bind", "0.0.0.0:${NGINX_PORT}", "kittygram_backend.wsgi"]
