FROM alpine:3.12
# https://www.iranvir.com/clang-on-alpine/

RUN apk upgrade && apk add clang lld libc-dev compiler-rt compiler-rt-static make cmake ninja meson git 

RUN adduser --disabled-password clang
USER clang
WORKDIR /home/clang

ENTRYPOINT ["/bin/ash"]
