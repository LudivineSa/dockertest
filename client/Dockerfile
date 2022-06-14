FROM node:lts-alpine

WORKDIR /app
# Cache and Install dependencies
COPY package.json .
COPY yarn.lock .
RUN yarn install
# Copy app files
COPY . .
# Expose port
EXPOSE 8080
# Start the app
CMD [ "yarn", "start" ]