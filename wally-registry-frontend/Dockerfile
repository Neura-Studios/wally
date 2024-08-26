FROM node:14.15
WORKDIR /app
EXPOSE 8000

COPY . /app

RUN npm install

ARG WALLY_API_URL
RUN cd /app && ls && exit -1
RUN npm run build

CMD ["node", "build/server/server.js"]
