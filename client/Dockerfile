FROM node:17-slim AS build

WORKDIR /usr/src/app
COPY package.json package-lock.json ./

# Install dependencies and copy them to the container
RUN npm install
COPY . .

# Run the web service on container startup.
CMD ["npm", "start"]
