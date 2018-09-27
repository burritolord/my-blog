FROM ghost:2-alpine

# Install mysql client and copy wait-for-it script
RUN apk add mysql-client
COPY wait-for-it.sh /usr/local/bin/wait-for-it.sh

# Change working directory to ghost root
WORKDIR /var/lib/ghost

# Copy dev config
COPY config.development.json .

# Copy prod config

# Copy my themes
COPY themes/uno-zen/ ./content/themes/