FROM node:carbon-alpine 

# ENV HOME .
# WORKDIR ${HOME}
WORKDIR app/
RUN apk add openssl
RUN npm i -g http-server

COPY . .

# RUN openssl req -x509 -sha256 -nodes \
#     -days 365 -newkey rsa:2048 -keyout key.pem -out \ 
#     cert.pem

#RUN apt-get install -y npm 
#&& \
 #   npm start

EXPOSE 8080
ENTRYPOINT sh start_script.sh

