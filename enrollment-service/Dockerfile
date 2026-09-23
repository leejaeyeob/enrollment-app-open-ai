FROM python:3.11-slim

WORKDIR /app

COPY enrollment-service/requirements.txt ./requirements.txt

RUN pip install --no-cache-dir -r requirements.txt

COPY enrollment-service ./enrollment-service
COPY prompts/service ./prompts/service
COPY prompts/lab4 ./prompts/lab4

EXPOSE 5001

CMD ["python", "enrollment-service/app.py"]
