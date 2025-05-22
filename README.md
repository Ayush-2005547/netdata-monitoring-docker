# Netdata Monitoring Dashboard (Docker)

This project sets up **Netdata**, a lightweight and powerful monitoring tool, using Docker. It allows real-time monitoring of system and application metrics via a web-based dashboard.

##  Objective
- Install Netdata via Docker
- Visualize real-time system performance (CPU, RAM, Disk, etc.)
- Understand basic server monitoring

## 🛠 Tools Used
- Docker
- Netdata (open-source system monitoring tool)

##  Setup Instructions

1. Ensure Docker is installed and running
2. Run the following command to start Netdata:

```bash
docker run -d --name=netdata -p 19999:19999 --cap-add=SYS_PTRACE --security-opt=apparmor=unconfined netdata/netdata
