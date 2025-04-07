FROM node:18-alpine AS development
ENV REACT_APP_BASE_URL=http://localhost:5000
EXPOSE 3000
WORKDIR /web
COPY package.json package-lock.json ./

RUN npm install
COPY . .

CMD [ "npm", "start" ]

RUN npm run build

