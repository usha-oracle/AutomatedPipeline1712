ARG version="18.04"
FROM ubuntu:$version
RUN echo "version..."$version
ARG licensekey="100..2000"
# First Dockerfile..
LABEL MAINTAINER us@oracle.com
RUN mkdir /code 
COPY sample.sh /code/sample.sh
COPY testfile /code/testfile
RUN chmod +x /code/sample.sh
RUN echo "Image is Built at `date`"
RUN echo "license key is .. "$licensekey
#ENTRYPOINT ["sh","/code/sample.sh"]
#CMD ["/code/testfile"]
CMD echo "Container being built"
CMD env
