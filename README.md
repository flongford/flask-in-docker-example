## Flask-in-Docker Example

Build the docker container using
```
build -t flask-in-docker:latest .
```

Then deploy the flask app in a container by invoking

```
docker run -d -p <host>:<port>:5000 flask-in-docker
```

The `host` and `port` variables define the external access ports to the docker container.
If left unspecified, you can identify them for a particular container by
using the `docker container list` command.

The app will now be running at:

```
http://<host>:<port>/
```

