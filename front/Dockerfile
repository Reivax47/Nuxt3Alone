#Front
FROM node:latest
RUN apt -y update
RUN apt -y upgrade
RUN apt-get -y install  vim


# Montage des documents partagés
COPY ./nuxt-app/ /root/front/
WORKDIR /root/front
RUN npm install
ENV NUXT_PORT=3000
CMD ["npm", "run", "dev"]

