FROM node:16.14-alpine

# Set environment variables for increased timeout and registry
ENV NPM_CONFIG_FETCH_TIMEOUT=60000
ENV NPM_CONFIG_CONNECT_TIMEOUT=60000
RUN npm config set registry https://registry.yarnpkg.com

# Optionally clear npm cache
RUN npm cache clean --force

WORKDIR /app-backend

COPY . .

RUN npm install --verbose

CMD ["npm", "start"]
