FROM node:20

RUN useradd -ms /bin/bash fenix

USER fenix

WORKDIR /home/fenix/code

COPY --chown=fenix index.js .

CMD ["node", "index.js"]
