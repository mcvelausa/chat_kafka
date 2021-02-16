#FROM balenalib/raspberry-pi-alpine-node:latest
FROM yobasystems/alpine-nodejs:arm32v7

# copy app source to destination container
COPY . .


# Install app dependencies
RUN npm install

#RUN npm install -g npm@7.5.4

#RUN npm audit fix --force

# expose container port
EXPOSE 3000

CMD npm start