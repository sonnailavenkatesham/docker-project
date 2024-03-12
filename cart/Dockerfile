FROM node:14
RUN useradd roboshop
USER roboshop
WORKDIR /app
COPY package.json /app
COPY server.js /app
RUN npm install
ENV REDIS_HOST=redis \
    CATALOGUE_HOST=catalogue 
CMD [ "node", "server.js" ]