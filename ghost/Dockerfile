FROM ghost:2-alpine

RUN apk update && apk upgrade

# Install tools to use in project
RUN npm install --global gulp-cli
RUN apk add --no-cache git

# Not sure why this does not work
# WORKDIR /var/lib/ghost/content/themes/uno-zen
# COPY content/themes/uno-zen/package.json .
# RUN npm install