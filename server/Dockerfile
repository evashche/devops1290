FROM node:14.17.3-alpine3.14
ENV PORT=5000
ENV CLIENT_PORT=3000
WORKDIR /server
EXPOSE 5000
COPY package.json package-lock.json ./
RUN npm install
COPY . ./
CMD ["npm", "start", "--", "--p", "$PORT", "--cp", "$CLIENT_PORT"]
