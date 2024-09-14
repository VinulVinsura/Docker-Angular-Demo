#use base image from docker hub
FROM node:20-alpine

#set the working directory
WORKDIR /app

#copy the package.json and package-lock.json file
COPY package*.json ./

#Install the dependencies
RUN npm install

#copy the rest of application file
COPY . .

#Export the port your app will run on
EXPOSE 4200

#start the application
CMD [ "ng" , "serve" ]