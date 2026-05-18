FROM node:18 AS build

WORKDIR /app
COPY frontend/package*.json ./
RUN npm install

COPY frontend/ .
EXPOSE 3000

CMD ["npm", "start"]
# FROM nginx:alpine
# COPY --from=build /app/build /usr/share/nginx/html

# EXPOSE 80