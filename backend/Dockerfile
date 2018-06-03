FROM node:10.0.0

MAINTAINER nodebotanist

# Install the npm packages which change infrequently
WORKDIR /extension/backend
COPY ./package.json ./
RUN npm install supervisor -g
RUN npm install

EXPOSE 8080
CMD ["./entrypoint.sh"]
