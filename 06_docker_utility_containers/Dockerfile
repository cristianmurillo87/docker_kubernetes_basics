# This docker file can be used to run an utility container
# which can be used to run Nodejs without having to install it
# in the pc.

# In this case, if run in interactive mode,
# npm will be executed after the container is started and the user can enter arguments for the command
# e.g init or install package1 package 2
# docker run -it -v "/Users/cristian/Documents/Udemy Courses/docker_course/docker_kubernetes_practical_guide/docker-utility-containers:/app" node-util init

FROM node:14-alpine

WORKDIR /app

ENTRYPOINT [ "npm" ]