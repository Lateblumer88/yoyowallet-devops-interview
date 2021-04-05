FROM python:3.6.1
RUN python3 -m pip install --upgrade pip
RUN python -m pip install --upgrade pip
RUN pwd
COPY **/*requirements.txt ./
COPY **/*run.py ./
RUN pip3 install pyjwt
RUN pip3 install jwt
RUN pip3 install -r ./requirements.txt
RUN export HTTP_PORT=5001
RUN export JWT_SECRET=supersecret
ENV HTTP_PORT=5000
ENV JWT_SECRET=supersecret
CMD ["python3","run.py"]