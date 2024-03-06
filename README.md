# dashboard

**Quick start project which will help in maintaining a development environment.**

--- 

### Running through Podman or Docker

> - For Docker container run this script: `build-docker.sh`
> - For Podman container run this script: `build-podman.sh`

### Multi Architecture

linux/arm64/v8
`docker build --platform linux/amd64 -t buildimages:latest -f Dockerfile --no-cache .`

### Docker Commands

> - Docker restart: `curl POST -H 'Content-Type: application/json' -d '{ "openContainerView": true }' -kiv --unix-socket ~/Library/Containers/com.docker.docker/Data/backend.sock http://localhost/engine/restart`
> - Docker certificate test: `openssl s_client -connect download.docker.com:443 -showcerts`
> - Docker login:  `docker login`
> - Docker start: `open --background -a Docker`
> - Check cpu info: `lscpu or lscpu | egrep 'Model name|Socket|Thread|NUMA|CPU\(s\)' or lscpu -p`
> - Docker log driver info: `docker info --format '{{.LoggingDriver}}'`


### Nginx and config

> - View the nginx configuration file: sudo nano /etc/nginx/nginx.conf <br>
> - Test the nginx configuration file: nginx -t <br>
> - Restart nginx: nginx -s reload <br>
> - Restart nginx on Linux: sudo systemctl restart nginx or sudo systemctl reload nginx <br>
> - Location of the nginx (error) logs: /var/log/nginx/error.log <br>
> - Check nginx service on Alpine: ps aux | grep "[n|N]ginx" or just pgrep nginx

### Prerequisites

> - Access to an AWS Account: https://eu-west-1.console.aws.amazon.com/console/home?region=eu-west-1 and the regions eu-west-1 and us-east-1.
> - A Mac or MacBook, this tool is only been tested with macOS.
> - A compatible browser like Safari, Firefox, Chrome, Edge, Opera or Yandex.
> - An IDE, this tool has only been tested with Intellij: https://www.jetbrains.com/.
> - AWS CLIv2: https://github.com/aws/aws-cli/tree/v2.
> - Go: https://go.dev/learn/.
> - Python: https://www.python.org/.
> - Granted: https://docs.commonfate.io/granted/getting-started/ `brew tap common-fate/granted` and `brew install granted`.
> - JQuery: https://api.jquery.com/.

### Optional

> - jq: https://stedolan.github.io/jq/ brew install jq.
> - AWS Boto3: https://github.com/boto/boto3.
> - AWK: https://formulae.brew.sh/formula/awk `brew install awk`.
> - Podman: https://podman.io/getting-started/installation.
> - Docker: https://docs.docker.com/desktop/install/mac-install/.
> - DockerHub: https://www.docker.com/products/docker-hub/.
> - SteamPipe: https://steampipe.io/downloads `brew install turbot/tap/steampipe`.

> #### [GitHub](https://github.com/RobertoTorino)
> ![GitHub](images/github.png) 
