FROM python:3.6.1-alpine
WORKDIR /usr/src/app
#ADD . /project
RUN python3 -m pip install --upgrade pip
RUN pwd
RUN ls
#COPY /var/lib/jenkins/workspace/YOYO-devops-interview-auth-api/auth-api/requirements.txt  /requirements.txt
COPY requirements.txt ./
RUN pip3 install -r requirements.txt
RUN export HTTP_PORT=5000
RUN export JWT_SECRET=supersecret
CMD ["python","run.py"]