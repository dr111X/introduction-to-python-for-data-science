# Python for Data Science Workshop (Spring 2019)

## Using Conda

Create the environment...

```bash
$ conda env create -f environment.yml
```

...then activate the newly created environment...

```bash
$ source activate $(head -1 $environment.yml | cut -d' ' -f2)
```

...then launch the notebook server.

```bash
$ jupyter notebook
```

## Using Docker

Pull the image from DockerHub...

```bash
$ docker pull kaustvl/introduction-to-python-for-data-science:spring-2019
```

...then run a container using the newly built image...

```bash
$ docker run --rm -v $(pwd):/home/al-khawarizmi/project -p 8888:8888 -it kaustvl/introduction-to-python-for-data-science:spring-2019
```

...inside the container the conda environment should already be activated so just launch the notebook server...

```bash
$ jupyter notebook --ip 0.0.0.0 --no-browser
```

...then open a browser on your local machine and copy and paste the provided link.


