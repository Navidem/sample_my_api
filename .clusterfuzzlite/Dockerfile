FROM gcr.io/oss-fuzz-base/base-builder:v1
RUN apt-get update && apt-get install -y make autoconf automake libtool
RUN COPY . $SRC/my-api-repo
WORKDIR my-api-repo
COPY .clusterfuzzlite/build.sh $SRC/
