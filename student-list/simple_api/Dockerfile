FROM python:2.7-stretch
LABEL maintainer=milica.djajic@hotmail.com
COPY . /
VOLUME /data
RUN yum update -y && yum install python-dev python2-dev libsasl2-dev python-dev libldap2-dev libssl-dev -y
RUN pip install flask==1.1.2 flask_httpauth==4.1.0 flask_simpleldap python-dotenv==0.14.0
EXPOSE 5000
CMD [ "python2", "./student_age.py" ]