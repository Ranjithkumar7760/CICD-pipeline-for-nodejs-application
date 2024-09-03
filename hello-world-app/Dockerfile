FROM node:16-alpine

WORKDIR /app

COPY package*.json ./

# Install dependencies with verbose logging and retry if it fails
RUN npm install --loglevel verbose || npm install --loglevel verbose --unsafe-perm

COPY . .

EXPOSE 3000

CMD ["node", "app.js"]