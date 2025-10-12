# Use Node base image
FROM node:18

# Set working directory
WORKDIR /app

# Copy dependency files
COPY package*.json ./
RUN npm install

# Copy the rest of the files
COPY . .

# Expose frontend port
EXPOSE 5173

# Run Vite dev server
CMD ["npm", "run", "dev", "--", "--host"]
