FROM node:20

WORKDIR /app

RUN apt-get update && apt-get install git -y
RUN git clone https://github.com/TheBigBrownBear/vitrine_back.git .

RUN npm install
ENTRYPOINT ["node", "server.js"]
