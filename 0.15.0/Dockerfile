FROM stackmachine/protobuf

# install protobuf from source
RUN apt-get update && \
    apt-get install -y curl git build-essential autoconf libtool
RUN git clone -b release-0_15 https://github.com/grpc/grpc && \
    cd grpc && \
    git submodule update --init && \
    make && \
    make install && \
    cd .. && rm -rf grpc

