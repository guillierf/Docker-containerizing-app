# Docker-containerizing-app

This example is taken from:
Pluralsight: Containerizing a Software Application with Docker

# single-stage image build
Build Docker image:
```
cd single-stage
docker build . -t nginx-single-stage
```
Run the Docker image:
```
docker run -d -p 80:80 nginx-single-stage:latest
```

# multi-stage image build
Build Docker image:
```
cd multi-stage
docker build . -t nginx-multi-stage
```
Run the Docker image:
```
docker run -d -p 80:80 nginx-multi-stage:latest
```
