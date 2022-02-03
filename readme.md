# hello-world-prometheus
Prometheus에 대한 hello world 프로젝트

## 1. Architecture overview


### 1.1 Software Version Info
- Prometheus: [v2.32.0](https://github.com/prometheus/prometheus/releases/tag/v2.32.0)
- Cadvisor: [v0.37.5](https://github.com/google/cadvisor/releases/tag/v0.37.5)
- Node-exporter: [v1.3.1](https://github.com/prometheus/node_exporter/releases/tag/v1.3.1)
- Grafana: [8.3.3](https://github.com/grafana/grafana/releases/tag/v8.3.3)

## 2. Install
Docker를 이용해 설치 및 실행하며 여러 docker image를 사용하기 때문에 docker-compose를 이용해 container를 관리한다.

## 2.4 Execution environment info
해당 프로젝트는 아래 환경에서 정상 동작했음을 테스트했다.
- OS: CentOS Linux release 7.8.2003 (Core)
- Kernel version: 3.10.0-1127.18.2.el7.x86_64 #1 SMP Sun Jul 26 15:27:06 UTC 2020
- Docker version: 20.10.5
- Docker-compose version: 1.28.6, build 5db8d86f

## 3. Configuration
이 프로젝트를 정상 설치 및 실행하기 위해 사용자 환경에 따라 기본적으로 변경되어야 하는 설정은 다음과 같다.

- Prometheus:
    - ./prometheus/sd_configs/file/*.yml
        - scrape target에 대한 endpoint(IP 및 PORT 정보) 설정 필요
        
- Grafana:

## 4. Documentation
- [Prometheus](https://prometheus.io/docs/introduction/overview/)
- [Cadvisor](https://github.com/google/cadvisor)
- [Node-exporter](https://github.com/prometheus/node_exporter)
- [Grafana](https://grafana.com/docs/grafana/latest/)

## 4. Etc
- Prometheus에 대한 고가용성(High Availability)을 위해 [Cortex](https://cortexmetrics.io/docs/)를 이용할 수 있으며 관련해서는 [hello-world-cortex]() 프로젝트 참고