#Dockerfile for flask containerization
FROM centos:centos7
MAINTAINER Brian Hopkins "brianhh1230@gmail.com"

RUN yum update -y
RUN yum -y install epel-release
RUN yum -y install python3-pip build-essentials python-dev
COPY . /app
WORKDIR /app
RUN pip3 install --upgrade pip
RUN pip3 install -r requirements.txt

ENTRYPOINT ["python"]
CMD ["app.py"]

