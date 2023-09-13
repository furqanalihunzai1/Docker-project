FROM node:alpine
WORKDIR /app

COPY package.json .
COPY package-lock.json ./

RUN npm install
RUN npm install bootstrap@4.6.0 reactstrap@8.9.0 --legacy-peer-deps
RUN npm install axios@0.21.1
ENV PATH /app/node_modules/.bin:$PATH
EXPOSE 3000
COPY . .
CMD ["npm", "start"]