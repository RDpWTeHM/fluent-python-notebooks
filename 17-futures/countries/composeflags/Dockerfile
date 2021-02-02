FROM nginx:alpine

WORKDIR /fluent_python/ch17/countries

RUN set -eux && sed -i 's/dl-cdn.alpinelinux.org/mirrors.ustc.edu.cn/g' /etc/apk/repositories
COPY nginx.conf /etc/nginx/conf.d/flags.conf
COPY flags.zip flags.zip
RUN unzip flags.zip
