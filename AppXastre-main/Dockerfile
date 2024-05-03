
FROM node:14


ENV DISPLAY=host.docker.internal:0.0


WORKDIR /app


COPY package*.json ./
COPY main.js ./
COPY app.js ./
COPY ./views ./views
COPY ./routes ./routes
COPY ./models ./models
COPY ./config ./config


RUN npm install


COPY . .


CMD ["npm", "start"]
