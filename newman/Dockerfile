FROM postman/newman:5

WORKDIR /etc/newman

COPY postman_collection.json .

RUN npm install -g newman-reporter-htmlextra
