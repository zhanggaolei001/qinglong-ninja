FROM whyour/qinglong:latest

RUN set -ex \
    && git clone https://github.com/MoonBegonia/ninja.git /ql/ninja \
    && cd /ql/ninja/backend \
    && pnpm install

COPY docker-entrypoint.sh /ql/docker/docker-entrypoint.sh
COPY sendNotify.js /ql/scripts/sendNotify.js

EXPOSE 5701

ENTRYPOINT ["./docker/docker-entrypoint.sh"]