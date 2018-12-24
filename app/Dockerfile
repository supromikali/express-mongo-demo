FROM node:10

# Create app directory
WORKDIR /usr/src/app

COPY package.json ./

# Install app dependencies
RUN npm install

# Copy app source
COPY . .

# Build app
RUN npm run build

EXPOSE 3000
CMD [ "npm", "start" ]