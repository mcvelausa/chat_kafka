#FROM balenalib/raspberry-pi-alpine-node:latest
FROM yobasystems/alpine-nodejs:arm32v7
<<<<<<< HEAD

# App
ADD . .


# Install app dependencies
RUN npm install

RUN npm install -g npm@7.5.4

RUN npm audit fix --force

EXPOSE  3000
CMD ["npm", "start"]
=======

# copy app source to destination container
COPY . .


# Install app dependencies
RUN npm install

#RUN npm install -g npm@7.5.4

#RUN npm audit fix --force

# expose container port
EXPOSE 3000

CMD npm start
>>>>>>> 745a400e61fceb3393834c446fccb0799245638a
