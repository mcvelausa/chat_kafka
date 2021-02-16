FROM balenalib/raspberry-pi-alpine-node:latest

# App
ADD . /chat-ui
# Install app dependencies
RUN cd /chat-ui; npm install

EXPOSE  4000
CMD ["npm start"]