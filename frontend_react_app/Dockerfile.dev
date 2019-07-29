# base image which contains node related to node modules
FROM  node:alpine


# specifying working directory
WORKDIR /app

# Copying package.json to docker filesystem
COPY ./package.json .

# Installed dependecies
RUN npm install

# Copying local files to docker filesystem
COPY . .

# command that runs when we create container
CMD ["npm", "start"]