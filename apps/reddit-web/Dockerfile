FROM node:19-alpine3.15

WORKDIR /reddit-clone

COPY package.json package-lock.json ./
RUN npm install 

COPY . .

RUN npm run build

EXPOSE 3000
CMD ["npm","run","start"]
