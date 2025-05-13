# Use official Node.js LTS image
FROM node:18

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

ENV PORT=5173
# Expose the frontend port (adjust if different)
EXPOSE 5173

# Start the frontend server (adjust if using a different script)
CMD ["npm", "run", "dev"]
