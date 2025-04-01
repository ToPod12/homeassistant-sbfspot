FROM alpine:latest
RUN apk update && apk add --no-cache git cmake build-base sqlite sqlite-dev
RUN git clone https://github.com/SBFspot/SBFspot.git /opt/SBFspot
WORKDIR /opt/SBFspot/SBFspot
RUN mkdir -p /opt/SBFspot/SBFspot/build
WORKDIR /opt/SBFspot/SBFspot/build
RUN cmake ..
RUN make
RUN make install
