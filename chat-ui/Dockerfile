FROM node:15.8.0-alpine
# Create app directory
WORKDIR /usr/src/docker-react-chat
# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json ./
RUN npm install -g npm@7.5.4
RUN npm -v
RUN node -v

#To bundle your app’s source code inside the Docker image, use the COPY instruction:
COPY ./public ./public
COPY ./src ./src

RUN ls -l
RUN npm install --production
#Your app binds to port 3000 so you’ll use the EXPOSE instruction to have it mapped by the docker daemon:
EXPOSE 3000
CMD ["npm", "start"]