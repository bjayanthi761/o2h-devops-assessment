# Troubleshooting Scenarios

## Scenario 1: Docker Container Exits Immediately

### Possible Reasons

- Application crashes on startup
- Incorrect CMD instruction
- Missing dependencies
- Port conflict
- Main process completed

### Debugging Steps

docker ps -a

docker logs <container-id>

docker inspect <container-id>

docker run -it o2h-app sh

---

## Scenario 2: Application Works Locally but Not on Server

### Checks

- Application logs
- Firewall rules
- Open ports
- Environment variables
- DNS settings
- Network connectivity

### Commands

ping <server-ip>

curl localhost:3000

netstat -tulnp

journalctl -xe
