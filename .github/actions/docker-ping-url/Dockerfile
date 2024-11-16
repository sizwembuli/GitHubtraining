FROM python:alpine3.11

WORKDIR /app

COPY requirements.txt

RUN python -V
RUN pip install --no-cache-dir -r requirement.txt

COPY . .

CMD [ "python", "/app/main.py"]