FROM node:24.14.1
COPY . /app-curso
WORKDIR /app-curso
RUN addgroup dev && adduser -S -G andre dev
USER andre
RUN apk add --no-cache python2 g++ make
RUN yarn install --production
CMD ["node", "/src/index.js"]
EXPOSE 3000
ENV API_URL=exemplo-para-adicionar-variavel-de-ambiente