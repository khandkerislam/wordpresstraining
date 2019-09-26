FROM node:12-alpine

WORKDIR /app

# Install Grunt globally

RUN npm i -g grunt-cli

# Copy package.json and install dependencies

COPY ["package.json", "./"]

RUN npm install

# Copy Gruntfile and tasks

COPY ["Gruntfile.js", "./"]

COPY ["tasks", "./tasks"]

# By default, build Gesso

CMD ["grunt", "gessoBuildStyles"]