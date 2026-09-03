FROM node
WORKDIR /myapp
COPY pcakage*.json .
RUN npm install
COPY . .
CMD ["node", "index.js"]
EXPOSE 80
