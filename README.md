# Task 7: Monitor System Resources Using Netdata

## 🎯 Objective
Install Netdata in Docker and visualize system + application performance metrics.

---

## ⚙️ Steps Followed
1. Pulled and ran Netdata container using Docker:
   ```bash
   docker run -d --name=netdata -p 19999:19999 \
     -v /var/run/docker.sock:/var/run/docker.sock:ro \
     netdata/netdata
