# docker-gitbucket
[![Build Status](https://travis-ci.org/prince-0203/docker-gitbucket.svg?branch=master)](https://travis-ci.org/prince-0203/docker-gitbucket)

Setup a container with [GitBucket](https://github.com/takezoe/gitbucket) installed.

## Usage

To run the container, do the following:

```
% docker run -d -p 8080:8080 -p 29418:29418 -v ${PWD}/gitbucket-data:/gitbucket prince-0203/gitbucket
```

You can see gitbucket running on http://localhost:8080/
You also see gitbucket data write out to "./gitbucket-data".

In order to access the git repository over SSH (port 29418), check settings below.

- GitBucket > Administration > System Settings > SSH access

## Building

To build the image, do the following:

```
% docker build github.com/prince-0203/docker-gitbucket
```

A prebuilt container is available in the docker index.

```
% docker pull prince-0203/gitbucket
```

## GitBucket's license
see https://github.com/gitbucket/gitbucket
