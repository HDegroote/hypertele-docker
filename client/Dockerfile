FROM node:20-slim
RUN apt-get -y update
RUN apt-get -y install git

RUN mkdir /etc/hypertele/
RUN npm i -g hypertele@1.1.1
ENTRYPOINT ["hypertele", "-i", "/etc/hypertele/keypair.json"]
