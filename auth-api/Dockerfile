FROM python:3.6.1-alpine
WORKDIR /project
ADD . /project
RUN pip3 install -r requirements.txt
RUN export HTTP_PORT=5000
RUN export JWT_SECRET=supersecret
CMD ["python","run.py"]