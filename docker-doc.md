

create a container so that you can get the container ID

```shell
docker create nginx
```

script way to do it

```shell
CID=$(sudo docker create nginx:latest)
echo $CID
```

using a container ID (CID) file:

> CID file can be shared easily

```shell
docker create --cidfile /tmp/web.cid nginx
```

inspect the file:

```shell
cat /tmp/web.cid
```

another way to get container ID

```shell
CID=$(docker ps -l -q)
```
> -l --latest
> -q --quiet
> --no-trunc to get full ID
