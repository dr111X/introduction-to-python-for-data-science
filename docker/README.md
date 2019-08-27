## Running the Docker image

The following command will run a container based on the image 
`kaustvl/introduction-to-python-for-data-science:fall-2019`. If you do not already have a local 
copy of the image, the image will be automatically downloaded from DockerHub.

```bash
$ docker container run \
  --rm \
  --tty \
  --volume ../data:/home/$USER/app/data \ 
  --volume ../bin:/home/$USER/app/notebooks \
  --volume ../src:/home/$USER/app/src \
  --publish 8888:8888 \
  kaustvl/introduction-to-python-for-data-science:fall-2019
```

## Using Docker Compose

It is quite easy to make a typo whilst writing the above docker commands by hand, a less error-prone approach is to use [Docker Compose](https://docs.docker.com/compose/). The above docker commands have been encapsulated into the `docker-compose.yml` configuration file and the following command can be used to bring up a container based on our image.

```bash
$ docker-compose up --build
```

When you are done developing, the following command tears down the networking inrastructure for the running container.

```bash
$ docker-compose down
```
