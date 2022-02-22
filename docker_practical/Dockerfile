#Base image as alpine 
FROM alpine:latest

#Install nodejs and npm 
RUN apk add --no-cache nodejs npm

#Working directory is /app
WORKDIR /app

#Copy all code to /app folder
COPY . /app

#Install dependency 
RUN npm install

#Expose port 
EXPOSE 5000

#env variable
ENV ENV_NODE=production

WORKDIR /app
ENTRYPOINT ["node"]
CMD ["server.js"]

