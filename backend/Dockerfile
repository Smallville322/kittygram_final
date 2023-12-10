FROM python:3.9-slim
WORKDIR /app
RUN apt-get update && apt-get install -y make
COPY . .
RUN pip install --upgrade pip
RUN pip install -r requirements.txt --no-cache-dir
CMD ["make", "run"]
