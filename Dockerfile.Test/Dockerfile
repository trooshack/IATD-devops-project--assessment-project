WORKDIR /app
COPY ../package.json ../package-lock.json ./
RUN npm ci
COPY ../src ./src
COPY ../tests ./tests
CMD ["npm", "test"]
