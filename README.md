
# neuraltalk2-camera
[Neuraltalk2](https://github.com/karpathy/neuraltalk2) is a fantastic tool based on Torch which uses neural networks to automatically caption images.

[neuraltalk2-web](https://github.com/jacopofar/neuraltalk2-web) is a repository offers a Dockerfile and a web interface to implement REST interface.

This repository combines WebRTC and neuraltalk2 to achieve a half real-time image captioning, the goal is to implement a web-base image captioning interface by user's camera.



Installation
===============

You only need Docker

for [Docker Install](https://docs.docker.com/engine/installation/)

and get the image by

docker pull newhandnew/neuraltalk2-camera


Usage
=======

docker run --name neuraltalk2-camera -p 5000:5000 newhandnew/neuraltalk2-camera

the docker image already contain the pretrain model

visit https://localhost:5000  (need to be https because of camera allowance)

![alt tag](https://raw.githubusercontent.com/newhandnew/neuraltalk2-camera/master/demo.png)

[live demo](https://13.88.253.60:5000/)

if you want to use GPU
-----------------------
by changing useGPU: '-1' to '0' and replace the pretrain model by [Neuraltalk2](https://github.com/karpathy/neuraltalk2), you will get a better performance.


P.S.
=====

If you want to use the code only, you need to type

npm install


The code is very ugly, need time to refine.


