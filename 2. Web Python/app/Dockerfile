FROM python:3.8-slim

WORKDIR /app

COPY app.py /app/

RUN pip install flask gunicorn

EXPOSE 8000

CMD ["gunicorn", "-b", "0.0.0.0:8000", "app:app"]
