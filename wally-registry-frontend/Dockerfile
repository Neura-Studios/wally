FROM node:14.15
WORKDIR /app
EXPOSE 8000

COPY wally-registry-frontend/ /app

RUN npm install

ARG WALLY_API_URL
RUN npm run build

CMD ["node", "build/server/server.js"]
