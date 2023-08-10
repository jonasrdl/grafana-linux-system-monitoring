### Setup

You can setup multiple "monitorings" here. For example one host machine (which the Grafana is running) and 2 other machines, that are being monitored.
On the host machine, you can use the whole `docker-compose.yml`, on the other machines, you can remove the grafana part.   
(You don't need multiple Grafana instances, the sense of this whole thing is to have one central instance, which can monitor multiple hosts.)

Prometheus is by default running on port `9090` (this is also configurable). Means you can just add a datasource for every machine you want to monitor.   

Example: IP:PORT => `http://ip:9090` .

### Usage

Grafana is running on: `http://localhost:3000`

Prometheus datasrouce URL is: `http://prometheus:9090`

Grafana import dashboard ID: `1860`

## Final result

![Example Screenshot](example.png)
