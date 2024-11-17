FROM python:alpine3.11

WORKDIR /app

COPY requirements.txt .

RUN python -V
RUN apt-get update && apt-get install -y libpq-dev build-essential
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

CMD [ "python", "/app/main.py"]