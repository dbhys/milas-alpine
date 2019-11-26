# milas-alpine

To build a base alpine image, alpine version is 3.9.
Contains  bash vim procps unzip curl busybox-extras ca-certificates,
in order to do some operations in container.
And default Timezone is "Asia/Shanghai"

## How to use it
##### 1. Write your Dockerfile like this:

```
FROM dbhys/milas-alpine:3.9
COPY ${your_dist_files} /deployments

EXPOSE ${your_port}
CMD ${your_commands}

```
##### 2. Build your image
```
build -t my-image:1.0.0 .
```