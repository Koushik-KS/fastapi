FROM python:3.11

WORKDIR /app

COPY packages /packages

RUN pip install --no-index --find-links=/packages fastapi uvicorn

COPY . .

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]