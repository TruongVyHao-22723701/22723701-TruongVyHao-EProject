# Base image nhẹ, cập nhật mới nhất
FROM node:20-alpine

# Set working directory
WORKDIR /app

# Copy package.json & package-lock.json
COPY package*.json ./

# Cập nhật npm & cài dependencies
RUN npm install --production

# Copy source code
COPY . .

# Expose port
EXPOSE 3000

# Start server
CMD ["node", "index.js"]
