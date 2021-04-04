FROM python:3.6.1-alpine
#WORKDIR /project
#ADD . /project
RUN python3 -m pip install --upgrade pip
#COPY /var/lib/jenkins/workspace/YOYO-devops-interview-auth-api/auth-api/requirements.txt  /requirements.txt
#RUN ls
COPY requirements.txt /tmp/
RUN pip3 install -r /tmp/requirements.txt
RUN export HTTP_PORT=5000
RUN export JWT_SECRET=supersecret
CMD ["python","run.py"]