FROM node:alpine3.20
WORKDIR /app
RUN addgroup -S dev && adduser -S -G dev marcos
RUN apk add --no-cache python3 g++ make
COPY . .
RUN chown -R :dev /app && chmod -R g+rwx /app
USER marcos
RUN yarn install --production
EXPOSE 3000
CMD ["node", "src/index.js"]