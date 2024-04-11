FROM python:3.8-slim
WORKDIR /app
COPY ./client_1/requirements.txt requirements.txt
RUN pip install --no-cache-dir --upgrade -r requirements.txt
COPY ./client_1/app /app
CMD ['uvicorn', 'main:app', '--host', '0.0.0.0', '--port', '80']
