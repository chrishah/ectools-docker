# ectools-docker

Docker image containing a full install of [ectools](https://github.com/jgurtowski/ectools), including MUMmer.

Details about the setup:
 - Ubuntu 18.04
 - Python 2.7.15rc1
 - [ectools](https://github.com/jgurtowski/ectools)
 - [MUMmer](https://github.com/mummer4/mummer) 4.0.0beta2


To use the container, do e.g.:
```bash
#Run partition.py from ectools
docker run -it -v $(pwd):/in/ -w /in --rm chrishah/ectools-docker partition.py

#Run Nucmer from MUMmer
docker run -it -v $(pwd):/in/ -w /in --rm chrishah/ectools-docker nucmer
```


