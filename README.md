# Docker_basics
Basics of Docker to kickstart using Docker

In this we will pull a docker image, load in on our local machine or virtual machine (If you are using) and then run the container.

``` docker pull alpine

docker images

docker run alpine ls -l

docker run alpine echo "Hello from alpine"

docker run alpine /bin/sh

docker run -it alpine /bin/sh

```
Alright, we completed a basic tutorial of docker creation and execution.
Now we will create a docker container which will publish a static webpage

docker run --name static-webpage -d -P dockersamples/static-site
The above command will host the static webpage on a random port.

We can also specify the port number on which we want the page to be hosted.

docker run --name static-webpage1 -d -d 8888:80 dockersamples/static-site
In this way we have hosted a webpage using docker containers.

