FROM node:alpine
WORKDIR /app
RUN mkdir ./frontend
RUN mkdir ./shared
COPY frontend/package.json ./frontend
COPY frontend/package-lock.json ./frontend
COPY ./frontend ./frontend
COPY ./shared ./shared
WORKDIR /app/frontend
RUN npm i
CMD ["npm", "run", "start"]