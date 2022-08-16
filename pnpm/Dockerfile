FROM node:16-alpine
LABEL author="yola"

RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.tuna.tsinghua.edu.cn/g' /etc/apk/repositories
RUN apk add --no-cache python2 g++ make \
    && corepack enable \
    && corepack prepare pnpm@7.9.1 --activate