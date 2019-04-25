# Citizen Health Cooperative DAO

## Build Instructions

For a test image:

```bash
> docker build -t coop -f ./build/package/Dockerfile 
> docker run -dit --name coop -p 3000:8080 coop
```

This will expose the service on http://localhost:3000

To stop the service:

```bash
> docker kill coop
```
