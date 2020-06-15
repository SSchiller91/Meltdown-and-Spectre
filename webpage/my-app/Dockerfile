# specify the node base image with your desired version node:<version>
FROM node:13.12.0-alpine
# replace this with your application's default port
EXPOSE 80/tcp
WORKDIR /Users/StephanSchiller/Documents/webpage/my-app
ENV PATH /Users/StephanSchiller/Documents/webpage/my-app/node_modules/.bin:$PATH
COPY package.json /Users/StephanSchiller/Documents/webpage/my-app
COPY package-lock.json /Users/StephanSchiller/Documents/webpage/my-app
RUN npm install -y --silent
COPY . /Users/StephanSchiller/Documents/webpage/my-app
CMD ["npm", "start"]