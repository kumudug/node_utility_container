# Creating a Node utility container

* Build
   - `docker build . -t node-util`
* Run 
   - When running we are gonna give he command to run
   - Add a bind mount
   - The idea is to npm init a project using the docker container inside of the host machine instead of installing node in the host machine
   - `docker run -it -v $(pwd):/app --rm node-util npm init`