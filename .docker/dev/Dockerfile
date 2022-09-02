FROM node:18

# Create and define the node_modules's cache directory.
WORKDIR /cache

# install app dependencies
COPY package.json .
COPY package-lock.json .
RUN npm install --silent

WORKDIR /app
ENV PATH /app/node_modules/.bin:$PATH
COPY . .
RUN mkdir -p node_modules/.cache && chmod -R 777 node_modules/.cache
RUN chown -R node node_modules
USER node
