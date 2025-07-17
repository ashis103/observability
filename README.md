**## Essential config files for Obsevability

1. Please create T2 instance from AWS 
2. sudo apt update 
3. sudo apt install docker.io
4. sudo apt install docker-commose-v2
5. sudo usermod -aG docker $USER && newgrp docker
6. mkdir ovserbility :: cd ovserbility
7. git clone http://github.com/ashis103/observability.git
8. cd observability
9. docker compose up - d
10. IP:9090   # promitheos site
11. Ip:8080  # CAadvisor**
12. rate(container_cpu_usage_secound_total{name="students-app"}[5m])   # Promitheous Query 

### Download the prometheus config file  
  
	wget https://raw.githubusercontent.com/prometheus/prometheus/main/documentation/examples/prometheus.yml**


### Download Loki Config 
	wget https://raw.githubusercontent.com/grafana/loki/v2.8.0/cmd/loki/loki-local-config.yaml -O loki-config.yaml

  
### Download Promtail Config

 
	wget https://raw.githubusercontent.com/grafana/loki/v2.8.0/clients/cmd/promtail/promtail-docker-config.yaml -O promtail-config.yaml

