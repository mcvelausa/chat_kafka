FROM balenalib/raspberry-pi-alpine-node:latest

# App
ADD . /chat-ui
RUN yum install -y -q npm
RUN npm audit fix --force
# Install app dependencies
RUN cd /chat-ui; npm install

EXPOSE  4000
CMD ["npm", "start"]