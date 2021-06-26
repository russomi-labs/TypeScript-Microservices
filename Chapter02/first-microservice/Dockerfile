#LATEST NODE Version -which node version u will use.
FROM node:14.17.1-alpine3.13

# Create app directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

#install depedencies
COPY package.json /usr/src/app
COPY package-lock.json /usr/src/app
RUN npm install

#bundle app src
COPY . /usr/src/app

CMD [ "npm" , "start" ]
