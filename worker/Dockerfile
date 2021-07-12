FROM node:12
ENV NODE_ENV=production
ENV MULT=true
ENV ADD=true
ENV PORT=3000
WORKDIR /usr/src/app
COPY ["package.json", "package-lock.json*", "npm-shrinkwrap.json*", "./"]
RUN npm install --production --silent && mv node_modules ../
COPY . .
EXPOSE 3000
CMD ["node", "main.js"]

