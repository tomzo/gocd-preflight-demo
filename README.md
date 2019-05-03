# GoCD preflight API demo

Supporting code for blog post at https://kudulab.io/posts/gocd-preflight-validation/

# Setup

This setup is using [Dojo](https://github.com/ai-traders/dojo) with [docker-compose driver](https://github.com/ai-traders/dojo#docker-compose-driver).
The `gocd-cli` is provided by [gocd-cli-dojo](https://github.com/gocd-contrib/docker-gocd-cli-dojo) docker image and GoCD server is the [official image]((https://github.com/gocd/docker-gocd-server)).

Assuming you already have a working docker, you can install dojo with:
```bash
DOJO_VERSION=0.5.0
wget -O dojo https://github.com/ai-traders/dojo/releases/download/${DOJO_VERSION}/dojo_linux_amd64
sudo mv dojo /usr/local/bin
sudo chmod +x /usr/local/bin/dojo
```

Then to setup GoCD server and linked docker container with gocd-cli run following command at the root of the project:
```
./tasks setup_gocd
```
