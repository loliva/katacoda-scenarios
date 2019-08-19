`docker search --filter "is-official=true" ubuntu`{{execute}}

`docker images`{{execute}}

`docker run -it --name ubuntu ubuntu bash`{{execute}}

`exit`{{execute}}

`docker ps -a`{{execute}}

`docker start ubuntu`{{execute}}

`docker ps -a`{{execute}}

`docker exec -it ubuntu bash `{{execute}}

`exit`{{execute}}

`docker ps -a`{{execute}}

`docker stop ubuntu`{{execute}}

`docker rm ubuntu`{{execute}}

`docker ps -a`{{execute}}
