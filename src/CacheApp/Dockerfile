    FROM python:3.7.3-alpine

    COPY requirements.txt .

    RUN pip install -U pip && pip install --user -r requirements.txt

    WORKDIR /app

    COPY app .

    EXPOSE 6379

    CMD ["python", "app.py"]