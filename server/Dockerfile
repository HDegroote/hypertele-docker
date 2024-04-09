# Note: build from the parent directory
FROM node:20-slim

RUN useradd hypertele
USER hypertele

COPY node_modules /home/hypertele/node_modules
COPY package-lock.json /home/hypertele/
COPY package.json /home/hypertele/

WORKDIR /home/hypertele

ENTRYPOINT ["./node_modules/.bin/hypertele-server", "--private"]
