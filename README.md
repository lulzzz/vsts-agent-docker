**Visual Studio Team Services agent**

This repository contains docker images for the Visual Studio Team Services (VSTS) agent that runs tasks as part of a build or release.

**Supported tags and Dockerfile links**


* ubuntu-16.04-php-node
 * PHP 7.2 with composer
 * Node.js 9.9.0 with npm 5.6.0
 * Grunt-Cli


**How to use these images**

```
docker run \
    -e VSTS_ACCOUNT=<team name> \
    -e VSTS_POOL="<pool>" \
    -e VSTS_TOKEN="<pat>" \
    -v /var/run/docker.sock:/var/run/docker.sock \
    -it \
    emishealth/vsts-agent-docker:ubuntu-16.04-php-node
```