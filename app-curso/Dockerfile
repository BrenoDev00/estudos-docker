FROM node:24.14.1
COPY . /app-curso
WORKDIR /app-curso
RUN yarn install --production
CMD ["node", "src/index.js"]
EXPOSE 3000