## Docker compose

> Docker compose is a separete `cli` that gets installed with docker, used to start up multipe docker containers. Automates some of the long-winded arguments we were passing to `docker run`

`docker run <image id>` === `docker-compose up`

`docker build .` === `docker-compose up --build`

`docker-compose up -d` - launch container in background.

`docker-compose down` - stop containers.

### docker-compose restart policie

`no` - never attempts to restart thid container if stops or crashes.

`always` - if containers stops **for any reason** always attempt to restart.

`on-failure` - only restart if code container stops with an error.

`unless-stopped` - always restart unless we forcibly stop it.

### container status w/ docker compose

`docker-compose ps`
