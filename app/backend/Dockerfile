FROM node:16.14-alpine

# Set environment variables for increased timeout and registry
ENV NPM_CONFIG_FETCH_TIMEOUT=60000
ENV NPM_CONFIG_CONNECT_TIMEOUT=60000

# Optionally clear npm cache

WORKDIR /app-backend

COPY . .

RUN npm install --no-audit

CMD ["npm", "start"]
