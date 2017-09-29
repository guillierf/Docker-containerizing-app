# Docker-containerizing-app

This example is taken from:

Pluralsight: Containerizing a Software Application with Docker.

The example shows how to compile NGINX source code in a container and then extract only the binary.

Then run the NGINX binary with a custom index.html file.


# single-stage image build
Build Docker image:
```
cd Build-Docker/single-stage
docker build . -t nginx-single-stage
```
Run the Docker image:
```
docker run -d -p 80:80 nginx-single-stage:latest
```

# multi-stage image build
Build Docker image:
```
cd Build-Docker/multi-stage
docker build . -t nginx-multi-stage
```
Run the Docker image:
```
docker run -d -p 80:80 nginx-multi-stage:latest
```
