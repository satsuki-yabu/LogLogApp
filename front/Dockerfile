FROM node:current-slim
WORKDIR /myapp
COPY package.json .
RUN npm install
CMD [ "npm", "start" ]
COPY . .
