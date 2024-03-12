FROM node:14.13-alpine
RUN useradd roboshop
USER roboshop
WORKDIR /app
COPY package.json /app
COPY server.js /app
RUN npm install
ENV MONGO=true
ENV MONGO_URL="mongodb://mongodb:27017/catalogue"
CMD ["node", "server.js"]