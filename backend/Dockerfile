#Stage 1
FROM node:14-alpine AS builder
# Create app directory
WORKDIR /usr/src/app
# Cache and Install dependencies
COPY package.json /usr/src/app/package.json
COPY package-lock.json /usr/src/app/package-lock.json
ENV NODE_ENV production
RUN npm install --${NODE_ENV}
# Copy app files
COPY . /usr/src/app

# Expose port
EXPOSE 5000 80
# Run the app
CMD ["npm", "run", "server"]