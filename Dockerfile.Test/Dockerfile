# Use a lightweight Node.js image
FROM node:20.12-alpine

# Set working directory inside the container
WORKDIR /app

# Copy only dependency files first (for better caching)
COPY ../package.json package-lock.json ./

RUN npm install

# Copy application source code
COPY ../src ./src

# Copy application source code
COPY ../tests ./tests

CMD [ "npm", "test" ]
