FROM node:10-alpine

# Create app directory
WORKDIR /app

COPY package.json ./

# Install app dependencies
RUN npm install

# Copy app source
COPY . .

# Build app
RUN npm run build

EXPOSE 3000
CMD [ "npm", "start" ]