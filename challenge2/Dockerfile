#Initializes node.js
FROM node:14

#Sets the working directory
WORKDIR /usr/src/app

#Copies package.json and its buddy
COPY package*.json ./

#Intalls the dependencies
RUN npm install

#Copies the rest of the files to the working directory
COPY . .

#Exposes the port the app will run on
EXPOSE 3000

#Starts the app
CMD ["npm", "start"]
