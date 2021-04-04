FROM python:3.6.1-alpine
RUN python3 -m pip install --upgrade pip
COPY **/*requirements.txt ./
COPY **/*run.py ./
RUN pip3 install -r ./requirements.txt
RUN export HTTP_PORT=5000
RUN export REDIS_URL=redis://127.0.0.1:6379/0
CMD ["python","run.py"]