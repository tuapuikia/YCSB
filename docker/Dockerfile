FROM maven:latest

ARG VERSION

RUN apt-get update && apt-get install wget tar -y && wget https://github.com/brianfrankcooper/YCSB/releases/download/$VERSION/ycsb-$VERSION.tar.gz -O /tmp/ycsb-$VERSION.tar.gz && tar xvzf /tmp/ycsb-$VERSION.tar.gz && rm -rf /tmp/ycsb-$VERSION.tar.gz

WORKDIR ycsb-$VERSION
