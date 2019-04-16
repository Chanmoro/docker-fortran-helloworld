# docker-fortran-helloworld
This is Fortran HelloWorld example with docker.

## Installation
1. Clone this repository and build docker image.
```
$ git clone https://github.com/Chanmoro/docker-fortran-helloworld.git
$ cd fortran-helloworld
$ docker build -t fortran .
```

## Usage
1 . Run Fortran docker environment with mount current dir to /app.
```
$ docker run -it --rm ${PWD}/.:/app -w /app fortran bash
```

2 . Compile COBOL source code.
```
(docker)$ gfortran -o hello_world hello_world.f
```

3 . Run compiled hello_world binary.
```
(docker)$ ./hello_world 
Hello World!
```

## Acknowledgments
Enjoy Fortran!
