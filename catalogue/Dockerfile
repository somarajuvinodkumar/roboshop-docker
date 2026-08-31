#FROM node:20
FROM node:20-alpine
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install 
ENV MONGO="TRUE" \
    MONGO_URL="mongodb://mongodb:27017/catalogue"
CMD ["node", "server.js"]