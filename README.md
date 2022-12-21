# Learn Docker

## Clone App

- Clone app repo:
```bash
git clone https://github.com/leanhvu21042001/learn-docker.git`
```

- Change directory:
```bash
cd learn-docker
```

### Build container and run

- Build Dockerfile:
```bash
docker build -t getting-started .
```

- Run app:
```bash
docker run -dp 3000:3000 getting-started
```

- [Click here to open App](http://localhost:3000)

### Stop and delete container
- Get the ID of the container by using the `docker ps` command:
```bash
docker ps
```

- Use the `docker stop` command to stop the container.
```bash
#Swap out `<the-container-id>` with the ID from docker ps
docker stop <the-container-id>
```

- Once the container has stopped, you can remove it by using the docker rm command.
```bash
docker rm <the-container-id>
```

## Pull Image and run
- Pull image:
```bash
docker pull leanhvu21042001/getting-started
```

- Show image downloaded
```bash
docker image ls
```
> You should see image name is **leanhvu21042001/getting-started**

- Run image
```bash
docker run -dp 3000:3000 leanhvu21042001/getting-started
```

- [Click here to open App](http://localhost:3000)
### [Stop and delete container](#stop-and-delete-container)
