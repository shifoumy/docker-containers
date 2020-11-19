FROM node:15.2.1-buster

RUN apt update
RUN apt upgrade -y

WORKDIR /code/

RUN npm install -g @angular/cli

EXPOSE 4200

ENTRYPOINT ["ng serve"]
