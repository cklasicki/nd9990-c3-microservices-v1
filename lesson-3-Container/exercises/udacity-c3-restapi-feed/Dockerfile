# set the base image
FROM node:12

# create app directory
WORKDIR /usr/src/app

# copy package.json AND package-lock.json
COPY package*.json ./

# install all dependencies
RUN npm ci

# copy rest of the code
COPY . .

# expose port 8080
EXPOSE 8080

# define a command that should be executed
CMD ["npm", "run", "dev"]