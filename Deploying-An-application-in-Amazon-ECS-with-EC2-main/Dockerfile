# use the official centos 7 base image
FROM centos:centos7
# install the Apache HTTP sever Package from the centos Repository
RUN yum install -y httpd
# copy the index.html file from the docker build context to the default apache doucment root directory in the container
COPY index.html /var/www/html/
# specify the command to run when the container starts, which starts the apache HTTp server in the fore fround
CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]
# expose port 80 to allow incomming HTTP traffic to the container
EXPOSE 80