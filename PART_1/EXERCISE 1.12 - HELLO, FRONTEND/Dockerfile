# We need ruby 3.1.0. I found this from Docker Hub
FROM node:16.2

EXPOSE 5000
WORKDIR /usr/src/app
COPY ./app .

# Compile by following instructions from README
RUN npm install
RUN npm install -g serve
RUN npm run build
CMD ["serve", "-s", "-l", "5000", "build"]