#Stage 1
FROM node:alpine AS builder

WORKDIR /app
# Cache and Install dependencies
COPY package.json .
COPY package-lock.json .
RUN npm install --production
# Copy app files
COPY . .

ARG REACT_BACK_API_URL
ENV PORT 3000
# Build the app
CMD ["npm", "run", "build"]

# Stage 2
# Bundle static assets with nginx
FROM nginx:1.21.0-alpine as production
LABEL maintainer="Saan-B"
# Copy built assets from builder
COPY --from=builder /app/build /usr/share/nginx/html
# Add your nginx.conf
COPY --from=builder /app/nginx_entrypoint.sh ./nginx_entrypoint.sh/
# Expose port
EXPOSE $PORT
# Start nginx
ENTRYPOINT /bin/sh -x ./nginx_entrypoint.sh && nginx -g 'daemon off;'
