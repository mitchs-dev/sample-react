FROM node:12.19.1
WORKDIR /app
ENV PATH /app/node_modules/.bin:$PATH
COPY package.json ./
#COPY package-lock.json ./
RUN npm install --only=prod
RUN npm install react-scripts@3.4.1 -g --silent
COPY . ./
CMD ["npm", "start"]
