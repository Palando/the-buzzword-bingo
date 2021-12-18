FROM node:gallium-alpine

RUN mkdir -p /backend
WORKDIR /backend

COPY package.json package-lock.json ./
RUN npm install

COPY . .

EXPOSE 8080

CMD ["npm", "run", "start:prod"]
