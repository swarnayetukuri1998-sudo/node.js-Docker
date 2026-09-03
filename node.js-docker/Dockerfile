FROM node:19-alpine as first-stage
WORKDIR /myapp
COPY package*.json .
RUN npm install
COPY . .


FROM first-stage as final
RUN npm install --production
COPY . .
CMD ["node", "index.js"]
EXPOSE 80
