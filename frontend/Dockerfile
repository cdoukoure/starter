FROM mhart/alpine-node:7
MAINTAINER thedevtom

ENV HOST 0.0.0.0

# Create app directory
RUN mkdir -p /app
COPY . /app

WORKDIR /app
# Expose the app port
EXPOSE 3000

RUN npm install
RUN npm run build

CMD ["npm", "start"]
