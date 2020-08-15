1. how to install docker on mac
https://medium.com/@yutafujii_59175/a-complete-one-by-one-guide-to-install-docker-on-your-mac-os-using-homebrew-e818eb4cfc3

2. how to run a simple go web docker 
https://www.liwenzhou.com/posts/Go/how_to_deploy_go_app_using_docker/

3. docker (python + django + nginx sample)
https://blog.csdn.net/qq_25639809/article/details/78958647


Problems:

virtualbox need to forward the port to mac (host), using virtualbox manager ui -> running default -> network -> advance -> portfowrding. 

Debug on docker container:

eval "$(docker-machine env default)" # optional for virtual box user, this is needed even when a new terminal window is opened
docker ps  # find out the container you want to ssh into
docker exec -it docker_compose_mysql_1 /bin/bash  #ssh into docker
