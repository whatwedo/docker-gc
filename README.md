# whatwedo/docker-gc

Run spotify/docker-gc as reccuring task.


## Running

The docker-gc container requires access to the docker socket in order to function, so you need to map it when running, e.g.:

```
docker run --rm -v /var/run/docker.sock:/var/run/docker.sock whatwedo/docker-gc
```

By default, docker-gc runned in a Docker container will run every 1800 seconds (30 minutes). In some cases you might need to change this setting. Set the CLEAN_PERIOD_SECONDS variable to override this default.
