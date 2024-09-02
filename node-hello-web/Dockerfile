FROM node:20-bullseye

WORKDIR /app

EXPOSE 3000

RUN apt update && \
    apt install git

RUN git clone https://github.com/kjc1998/K8s.git && \
    cd /app/K8s/node-hello-web && \
    npm ci

WORKDIR /app/K8s/node-hello-web

CMD ["npm", "start"]