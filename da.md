# Create the index.html

# dockerFile
```
FROM nginx:alpine
COPY ./index.html /usr/share/nginx/html/
EXPOSE 80
```

#In docker App
- `docker build -f Docker -t mydocker .`
- `docker run -d -p 3000:80 mydocker`
- `docker ps`
- `docker stop`
- `docker ps`
- `docker tag mydocker:latest himaja14/mydocker:latest`
- `docker push himaja14/mydocker:latest`
