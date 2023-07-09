#Stage 1
FROM node:14-alpine AS builder
# App directory
WORKDIR /app

# App dependencies
COPY package*.json ./

# Copy app source code
COPY . .
ENV NODE_ENV dev
RUN npm install --${NODE_ENV}
# Copy app files
COPY . /usr/src/app

# Expose port
EXPOSE 5000
# Run the app
CMD ["npm", "start"]