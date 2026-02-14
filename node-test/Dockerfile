FROM node:18-alpine

WORKDIR /app

# Copy package files and install everything (including dev deps for testing)
COPY package*.json ./
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose port
EXPOSE 3000

# Start the app
CMD ["node", "index.js"]
