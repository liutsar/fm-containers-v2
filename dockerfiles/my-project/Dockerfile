FROM node:20

RUN useradd -ms /bin/bash fenix

USER fenix

WORKDIR /home/fenix/code

COPY --chown=fenix . .

EXPOSE 8080

RUN npm ci

CMD ["node", "index.js"]
