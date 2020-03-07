FROM node:alpine
LABEL maintainer="tinhcao <caodangtinh@gmail.com>"
WORKDIR /app
COPY ./package.json ./
RUN npm i
COPY ./ ./
EXPOSE 4200
CMD [ "npm","start" ]