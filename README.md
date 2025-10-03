# Monitor-System-Resources-Using-Netdata
Monitor System Resources Using Netdata in Docker container
# Monitor System Resources Using Netdata

##  Objective
Install and run **Netdata** to visualize and monitor system and application performance metrics in real time.

---

##  Tools
- **Netdata** → Free, open-source monitoring tool
- **Docker** → To run Netdata container

---

##  Steps to Run

### 1. Run Netdata in Docker
```bash
docker run -d --name=netdata \
  -p 19999:19999 \
  --cap-add SYS_PTRACE \
  --security-opt apparmor=unconfined \
  netdata/netdata
