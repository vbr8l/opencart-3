# HW CMS opencart-3
## Steps:
* git clone [opencart-3](https://github.com/vbr8l/opencart-3.git)
* cd opencart-3
* docker-compose build
* docker-compose up
* opencart-my-store - Web Store UI
* opencart-my-store/admin - Admin UI
* http://localhost:9090 - Prometheus UI
* http://localhost:9093 - Alertmanager UI
* http://localhost:8428 - VictoriaMetrics UI
* http://localhost:3000 - Grafana (default user/pass)
  - Dashboards, datasource, alerting provisioning
  - Infra cumulative dashboard (drill down dashboard) has links to another dashboards (MySQL, PHP-FPM, Nginx)
