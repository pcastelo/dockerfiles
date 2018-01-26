# How to use

[Redis Desktop Manager](https://redisdesktop.com/) on docker. Enjoy !

```bash
docker run  -it --rm \
    -v /tmp/.X11-unix:/tmp/.X11-unix \
    -v $HOME/.rdm:/root/.rdm \
    -e DISPLAY \
    --device /dev/dri \
    -e SSH_AUTH_SOCK \
    -v $SSH_AUTH_SOCK:$SSH_AUTH_SOCK \
    --name redis-desktop-manager \
    redis-desktop-manager
```

Nota1: Usar el nombre de la imagen buildeada
Nota2: para activar ui correr xhost +local:docker > /dev/null 
