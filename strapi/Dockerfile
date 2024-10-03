# Docker file inspired from https://docs.strapi.io/dev-docs/installation/docker#production-dockerfile

FROM node:20-alpine
ARG NODE_ENV=production

# Installing libvips-dev for sharp Compatibility
RUN apk update && apk add --no-cache chromium build-base gcc autoconf automake zlib-dev libpng-dev vips-dev git && rm -rf /var/cache/apk/* > /dev/null 2>&1
ENV CHROME_BIN="/usr/bin/chromium-browser" \
    PUPPETEER_SKIP_CHROMIUM_DOWNLOAD="true"
