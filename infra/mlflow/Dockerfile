FROM python:3.12-slim

# Install dependencies in a single layer
RUN pip install --no-cache-dir \
    mlflow==3.15.1 \
    "psycopg[binary]" \
    psycopg2-binary==2.9.12 \
    boto3==1.40.45

EXPOSE 5000

CMD ["mlflow", "server", "--host", "0.0.0.0", "--port", "5000"]