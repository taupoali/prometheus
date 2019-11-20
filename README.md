# Getting Started with Prometheus & Grafana
Config required for prometheus on Docker
When getting started with Prometheus and you just want to try it out in a non-production environment, you want a quick way to get up and running. The prom image gives us that. But there are a couple of things that need configured, such as the node exporter and maybe nicer visualization in Grafana. So the docker-compose file here is from 

https://linoxide.com/containers/setup-monitoring-docker-containers-prometheus/

There were some formatting issues with the source, so they are corrected in this repo

just pull this repo and you'll get the docker-compose.yaml file that will create a Prometheus container, a node-exporter container and Grafana container.

You will need to modify the prometheus.yml file to match the IPv4 address of your chosen Docker host.
The admin password for Grafana is controlled in the docker-compose.yml as an environment variable

Happy metric collecting!
