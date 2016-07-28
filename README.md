# digits-platform

Digits is still very much *in progress*, visit [the wiki](https://github.com/Digits-Project/digits-platform/wiki) for stuff and things.

We've started development, you can follow along with the commands below. NOTE: You need to have Docker installed for this to work. Check out [Docker for Mac](https://docs.docker.com/docker-for-mac/) or [Docker for Windows](https://docs.docker.com/docker-for-windows/) for an easy-to-install version of Docker for desktop machines.

To build the pgh.digits.pub webserver

```
cd pgh-digits-pub
docker build -t pgh-digits-pub .
```

Now that you have built the Docker image `pgh-digits-pub` you can run it on your local machine with the following command:

```
docker run --name pgh-digits-pub -d -p 8080:80 pgh-digits-pub
```

Now you can visit [http://localhost:8080](http://localhost:8080) and see Digits!
