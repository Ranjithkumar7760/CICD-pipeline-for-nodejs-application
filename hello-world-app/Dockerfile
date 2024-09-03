FROM node:14

WORKDIR /app

COPY package*.json ./

# Clear npm cache (optional)
RUN npm cache clean --force

RUN npm install

COPY . .

EXPOSE 3000

CMD ["npm", "start"]
