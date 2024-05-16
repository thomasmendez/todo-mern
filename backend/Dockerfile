FROM node:22-alpine3.18

WORKDIR /app

COPY package*.json ./

# Install the dependencies
RUN yarn install

# Copy the rest of the application code
COPY . .

RUN yarn build

# Expose the port the app runs on
EXPOSE 3000

# Run the application
CMD ["yarn", "start"]
