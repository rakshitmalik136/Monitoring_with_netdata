# Task 7: Monitor System Resources Using Netdata

## Objective
Install Netdata and visualize system and app performance metrics.

## Tools
- Netdata (Free, open-source monitoring tool)
- Docker

## Deliverables
- Screenshot of the dashboard and running metrics

## Steps to Run Netdata

### 1. Run via Docker
```bash
docker run -d   --name=netdata   -p 19999:19999   --cap-add SYS_PTRACE   --security-opt apparmor=unconfined   netdata/netdata
```

### 2. Access Netdata Dashboard
Open your browser and visit:
```
http://localhost:19999
```

### 3. Monitor Resources
- CPU usage
- Memory usage
- Disk usage
- Docker containers performance
- Alerts and chart panels

### 4. Explore Logs
You can find Netdata logs in:
```
/var/log/netdata
```

## Outcome
By completing this task, you will understand lightweight monitoring for servers or applications using Netdata.
