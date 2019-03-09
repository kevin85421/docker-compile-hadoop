# Compile hadoop in Docker container  
*   This image is the combination of [docker-hadoop](https://github.com/angelcervera/docker-hadoop) and [compile-hadoop](https://github.com/kiwenlau/compile-hadoop).
*   **Compile hadoop 2.7.1** in docker container.
*   This image is suitable for people who want to modify the hadoop source code (e.g. me lol)!

# HOW TO START A CONTAINER ?
##  Step1 : Clone this repo
##  Step2 : Download hadoop source code
```
cd docker-compile-hadoop-master
wget http://archive.apache.org/dist/hadoop/core/hadoop-2.7.1/hadoop-2.7.1-src.tar.gz
tar -xzvf hadoop-2.7.1-src.tar.gz
```
##  Step3 : Build the image
```
docker build  -t my-hadoop/hadoop-docker:2.7.1 .
```
## Step4 : Start the container
```
docker run -itd  my-hadoop/hadoop-docker:2.7.1 bash 
```
# Feel free to contact with me! Enjoy it!
