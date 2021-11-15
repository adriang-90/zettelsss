# Beginner Boost Container

Step by step instruction to create a basic container with linux and stuff.

1. *docker run -it --name boost -h boost ubuntu*
1. detach/attach from running container
    1. *ctrl+pq*
    1. docker attach boost
    1. detach quits the container but doesnt stop it, like *exit* command. In that case docker start "$name" is needed first before attach.
1. inside a container
    1. unminimize 
    1. apt update
    1. apt install nvi
    1. apt install vim
    

