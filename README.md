# dagLogo workshop

![.github/workflows/push_docker.yaml](https://github.com/jianhong/trackViewerBiocAsia2020Workshop/workflows/.github/workflows/push_docker.yaml/badge.svg)

[github page](https://jianhong.github.io/trackViewerBiocAsia2020Workshop/) | 
[source code](https://github.com/jianhong/trackViewerBiocAsia2020Workshop)

This package will create the docker file for the tools used for trackViewer, the sample code and files to run the pipeline, and
the slides for the course.

## Pre-requisites
* Basic knowledge of R
* Basic knowledge of Docker
* A computer with internet connection

## docker file
docker file for trackViewer

Dockerfile to build trackViewer 
Based on bioconductor_docker:devel

<pre>
$ cd ~
$ docker pull jianhong/trackviewerbiocasia2020workshop:latest
$ mkdir tmp4trackViewer
$ docker run -e PASSWORD=123456 -p 8787:8787 \
$       -v ${PWD}/tmp4trackViewer:/volume/data \
$       jianhong/trackviewerbiocasia2020workshop:latest

</pre>

## Learning goals

1. Gain the basic knowledge of typical workflows for trackViewer

2. Plot a lolliplot

3. Plot a dandelion
