FROM python:3.6

# Create app directory
RUN mkdir /usr/src/app
WORKDIR /usr/src/app

# Install app dependencies
COPY src/requirements.txt ./
RUN pip install -r requirements.txt

# Bundle app source
COPY src ./

EXPOSE 8080
CMD [ "python", "server.py" ]