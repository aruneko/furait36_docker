FROM alpine AS build-sl
RUN apk --no-cache add alpine-sdk ncurses-dev && \
    git clone https://github.com/mtoyoda/sl.git && \
    cd sl && \
    make

FROM alpine
RUN apk --no-cache add ncurses
COPY --from=build-sl /sl/sl /usr/bin/sl
