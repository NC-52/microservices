FROM node:12
# Create app directory
WORKDIR /usr/src/app
# Install all dependencies
# A wildcard is used nto ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json ./
RUN npm ci
# Bundle app source
COPY . .
EXPOSE 8080
CMD [ "npm", "run", "prod" ]
