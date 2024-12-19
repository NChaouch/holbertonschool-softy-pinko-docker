# Use the last picture Ubuntu like a basic
FROM ubuntu:latest
# Update packages and install python3 and pippython3
RUN apt-get update && apt-get install -y python3 python3-pip
# delete file
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED
# install flask with pip3
RUN pip3 install flask
# define repo
WORKDIR /app
# paste file api.py on file docker
COPY ./api.py /app/api.py
# command to execute
CMD ["python3", "api.py"]
