FROM node:alpine

WORKDIR /front

COPY library_front/package.json /front

COPY library_front/ /front/

RUN npm install


CMD ["npm", "start"]
EXPOSE 3000