# Use a lightweight Node.js image
FROM node:20.12-alpine

# Set working directory inside the container
WORKDIR /app

COPY ../ ./

RUN npm install

CMD [ "npm", "test" ]
