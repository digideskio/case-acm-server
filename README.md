# case-acm-server
Code and issues for the ACM docker server

## Overview
This uses docker-compose and systemd along with a couple short bash scripts to start and stop services running in docker containers.

## Requirements
Things are a bit specific to the ACM server's set up for now, so this will be rather un-flexable.

1. docker-compose in /usr/local/bin
2. YAML configs and net_*.sh scripts in /srv/acm/
3. acm@.server in /etc/systemd/system/
4. A folder for each service with the same name as the service, containing necessary *.env files and a single file called MAC with the services' container's mac address (as registered w/ CWRU ITS).
