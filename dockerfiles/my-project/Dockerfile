FROM node:20

RUN useradd -ms /bin/bash fenix

USER fenix

WORKDIR /home/fenix/code

COPY --chown=fenix:fenix package*.json ./

RUN npm ci

COPY --chown=fenix . .

CMD ["node", "index.js"]
