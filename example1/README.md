
# nginx example

Pull image

```
docker pull nginx:alpine
```

Run container

```
docker run --name example1 -p 8000:80 nginx:alpine
```

Remove container

``` 
docker rm -f example1
```

Run container in detached mode
```
docker run --name example1 -p 8000:80 -d nginx:alpine
```

Mount html as volume

```
docker run --name example1 -p 8000:80 -d 
-v /Users/ts/www/presentation/example1/html:/usr/share/nginx/html nginx:alpine
```

_Changes on index.html are reflected instantly_