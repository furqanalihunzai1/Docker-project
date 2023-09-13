FROM python:3.7-slim
ENV PYTHONUNBUFFERED=1
ENV PYTHONFONYWRITEBYTECODE=1

WORKDIR /app

RUN apt-get update \
    && apt-get install -y binutils libproj-dev \
    && apt-get install -y build-essential libpq-dev \
    && rm -rf /var/lib/apt/list/*


COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
CMD python manage.py runserver 0.0.0.0:8000