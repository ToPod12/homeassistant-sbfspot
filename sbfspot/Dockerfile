FROM ghcr.io/home-assistant/amd64-base:latest
RUN apk update && apk add --no-cache git cmake build-base sqlite sqlite-dev
RUN git clone https://github.com/SBFspot/SBFspot.git /opt/SBFspot \
    && cd /opt/SBFspot/SBFspot \
    && mkdir build && cd build \
    && cmake .. \
    && make \
    && make install
