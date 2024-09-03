FROM node:14

WORKDIR /app

COPY package*.json ./

# Clear npm cache (optional)
RUN npm cache clean --force

COPY . .

EXPOSE 3000

CMD ["npm", "start"]
