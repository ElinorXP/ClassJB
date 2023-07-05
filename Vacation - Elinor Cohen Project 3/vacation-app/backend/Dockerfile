FROM node:alpine
WORKDIR /app
RUN mkdir ./shared
RUN mkdir ./backend
COPY package.json ./backend
COPY package-lock.json ./backend
COPY ./ ./backend
WORKDIR /app/backend
COPY shared ../shared
RUN npm i
CMD ["npm", "run", "start"]