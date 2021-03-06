
# Docker-Sample

This repo is to run an index.html using a docker container.

## Installation

install apache, Docker

apache:https://www.digitalocean.com/community/tutorials/how-to-install-the-apache-web-server-on-ubuntu-20-04

Docker:https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04

build the docker file:

```bash
docker build -t="mywebserver" .
```
Here tag_name in our case is mywebserver:

webserver file has built, the next step is to create a container from the image for that we use the docker run command:
```bash
docker run -d -p 8080:80 tag_name
```

use below command as 80 port is already exposed:
```bash
docker run -d tag_name
```
or

```bash
docker run -d -p 80:80 tag_name
```
## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
