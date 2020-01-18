# Docker
Create Docker file Sample tutorial.
--------------------------------------

1. create directory where you want to place Dockerfile

`mkdir /Docker/sample`

`touch /Docker/sample/Dockerfile`

Add below list of line into Dockerfile. 

`FROM ubuntu:18.04`
`RUN apt-get update`
`RUN apt-get -y install nano`
`RUN apt-get -y install curl`

Now build a Docker image from this Dockerfile.

`cd /Docker/sample`

`docker build -t uffizio/sample:1.0 .`

This will create Docker image with the instructions you have given into Dockerfile.
you can list the created images with,

`docker images`

Rename Docker image.

`docker tag $image_id username/$image_name:$tag_name`

for example,

`docker tag df3ghfd32dftr5 purval/sample_image:version1`



