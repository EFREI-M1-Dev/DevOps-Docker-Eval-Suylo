FROM node:20

# Par défaut, on se place dans le dossier /app
WORKDIR /app

# ON update et on installe git
RUN apt-get update && apt-get install -y git

# On clone le repo
RUN git clone https://github.com/TheBigBrownBear/vitrine_front.git .

# On installe la dépendance serve (un peu comme nginx mais pour pour du node)
RUN npm install -g serve

CMD ["serve", "-s", ".", "-l", "80"]