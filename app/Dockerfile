FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json (if present)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose port 3000 (ensure your app listens on port 3000)
EXPOSE 3000

# Run the application
CMD ["node", "app.js"]
