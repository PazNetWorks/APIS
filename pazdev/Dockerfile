FROM python:3.8-slim
WORKDIR /app
COPY ./pazdev/requirements.txt requirements.txt
RUN pip install --no-cache-dir --upgrade -r requirements.txt
COPY ./pazdev/app /app
CMD ['uvicorn', 'main:app', '--host', '0.0.0.0', '--port', '80']
