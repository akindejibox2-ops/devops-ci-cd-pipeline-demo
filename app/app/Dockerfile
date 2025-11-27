# Step 1: Use Node official image
FROM node:18

# Step 2: Set working directory
WORKDIR /app

# Step 3: Copy package files first (for faster Docker caching)
COPY app/package*.json ./

# Step 4: Install dependencies
RUN npm install

# Step 5: Copy the rest of the app code
COPY app .

# Step 6: Expose port
EXPOSE 3000

# Step 7: Start the application
CMD ["npm", "start"]
