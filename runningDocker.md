

## Build & Run Docker Image

```bash
docker build -t <image-name> . 

docker run --name <container-name> -d <image-name>
```

## Attach to container

```bash
docker exec -it <container-name> bash
```

## Copy aws cred to container to use boto3
```bash
docker cp ~/.aws <container-name>:/root
```