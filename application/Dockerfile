FROM node:latest
WORKDIR /code
COPY package.json /code/package.json
COPY package-lock.json /code/package-lock.json
RUN npm install
COPY . .
RUN npm run build
EXPOSE 3000
CMD ["node", "build/index.js"]