FROM python:3.15.0a8-slim-trixie 
WORKDIR /app
COPY app.py /app/app.py
RUN apt-get update && apt-get install -y \
    iputils-ping 
CMD ["python", "app.py"]