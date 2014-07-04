# docker-gitbucket

Dockerfile for [gitbucket](https://github.com/takezoe/gitbucket)

# Usage

## From the docker repository

```
sudo docker pull stumpy/gitbucket
mkdir data
sudo docker run -d -p 8080:8080 -v `pwd`/data:/data:rw stumpy/gitbucket
```

if you want/need ssh access
```
sudo docker run -d -p 2022:22 -p 8080:8080 -v `pwd`/data:/data:rw stumpy/gitbucket
```


## From the Dockerfile

```
git clone https://github.com/stumpyfr/docker-gitbucket.git
cd docker-gitbucket
sudo docker build -t stumpy/gitbucket .
mkdir data
sudo docker run -d -p 8080:8080 -v `pwd`/data:/data:rw stumpy/gitbucket
```

if you want/need ssh access
```
sudo docker run -d -p 2022:22 -p 8080:8080 -v `pwd`/data:/data:rw stumpy/gitbucket
```


