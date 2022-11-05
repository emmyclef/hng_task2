FROM node:19-alpine3.15
WORKDIR /frontend
COPY . .
RUN npm install
RUN npm run build
EXPOSE 3000
RUN npm install -g serve
CMD ["serve", "-s", "build"]