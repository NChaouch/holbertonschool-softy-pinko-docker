# Use the last picture Ubuntu like a basic
FROM ubuntu:latest
# Update packages and install python3 and pippython3
RUN apt-get update && apt-get install -y python3 python3-pip
# delete file
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED || true
# install flask with pip3 and flask cors
RUN pip3 install flask flask-cors
# define repo
WORKDIR /app
# paste file api.py on file docker
COPY ./api.py /app/api.py

EXPOSE 5252
# command to execute
CMD ["python3", "api.py"]