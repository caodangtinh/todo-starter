FROM node:alpine as first_step
LABEL maintainer="tinhcao <caodangtinh@gmail.com>"
WORKDIR /app
COPY ./package.json ./
RUN npm i
#RUN npm i -g @angular/cli@8.3.21
COPY ./ ./
EXPOSE 4200
CMD [ "npm", "start" ]
#RUN ng build --prod

#second step of nginx
#FROM nginx:latest
#COPY --from=first_step /app/dist /usr/share/nginx/html
#COPY ./nginx.conf /etc/nginx/conf.d/default.conf