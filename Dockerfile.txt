# Use Python base image
FROM python:3.9-slim

WORKDIR /app

COPY app.py /app

# Install Flask
RUN pip install Flask

EXPOSE 5000

CMD ["python", "app.py"]

