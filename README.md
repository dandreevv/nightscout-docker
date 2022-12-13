# Personal Nightscout in one touch
Based on Nightscout, MongoDB and Traefik official docker images.

## Requirenments
- [Docker](https://www.docker.com) 

#### Optional
- Domain name

## Run
1. [Install Dcoker](https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository)
2. Change the settings
    - [nightscout.env](#nightscoutenv)
    - [docker-compose.yml](#docker-composeyml)
3. Run the services:
    - `sudo docker compose up -d`

## Config files
### nightscout.env
Here you can configure Nightscout.
Description of each parameter you can find on [official site](https://github.com/nightscout/cgm-remote-monitor#environment)

Important to change:
- API_SECRET: the password for Nightscout
- BASE_URL: Server domain name or IP

### docker-compose.yml
- You have not Domain name
    - Comment out or delite lines 21-49
    - Uncomment lines 19-20

- You have domain name
    - On line 24 put your Domain name
    - On line 43 put your email

