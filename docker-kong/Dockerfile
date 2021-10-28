FROM kong:2.3.2-alpine

LABEL description="Alpine + Kong 2.3.2 + kong-oidc plugin"

USER root
RUN apk update && apk add git unzip luarocks
RUN luarocks install --pin lua-resty-jwt 0.2.2-0
RUN luarocks install kong-oidc

USER kong