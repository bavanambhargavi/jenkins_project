# Filename :Dockerfile
FROM python:3.10.7 AS build
LABEL maintainer = "bhargavi"

# Any working directory can be chosen as per choice like '/' or '/home' etc
# i have chosen /usr/app/src
WORKDIR  D:\work_projects\
# WORKDIR  /usr/app/src

#to COPY the remote file at working directory in container
# ADD  

# Now the structure looks like this '/usr/app/src/test.py'

# RUN pip install --no-cache-dir -f file.txt
# RUN pip install python
RUN pip install pytest

COPY . . 


#CMD instruction should be used to run the software
#contained by your image, along with any arguments.
EXPOSE  50000

EXPOSE  8080

CMD [ "pytest", "start"]