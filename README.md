# docker-fortran-helloworld
This is Fortran HelloWorld example with docker.

## Setup
Clone this repository and build docker image.
```
$ git clone https://github.com/Chanmoro/fortran-helloworld.git
$ cd fortran-helloworld
$ docker build -t fortran .
```

## Usase
```
# 1. Run gfortran environment (docker).
# Mount current dir to /app.
$ docker run -it --rm ${PWD}/.:/app -w /app fortran bash

# 2. Compile fortran source code.
$ gfortran -o hello_world hello_world.f

# 3. Run compiled hello_world binary.
$ ./hello_world
>  Hello World!
```
