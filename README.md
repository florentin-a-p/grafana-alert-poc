# grafana-alert-poc

The goal of this project is to create a way to output alerts from Prometheus Alertmanager that is easily understood and managed by Product Managers.

Integrations include:
- Google Spreadsheets
- Notion

## How to run
```
docker compose up
```

The way to test it is to refresh `http://localhost:8090/ping` at least 6 times and then you will see the following alert at `http://localhost:9090/alerts`
<img width="1130" alt="image" src="https://github.com/florentin-a-p/grafana-alert-poc/assets/52971362/8c37b251-bc56-478b-9845-de46b80b34fa">

After that, you should see some alerts hitting your webhook URL like below
<img width="891" alt="image" src="https://github.com/florentin-a-p/grafana-alert-poc/assets/52971362/37f9ceb7-e924-4a96-9faf-3a9671f9ae95">


## References
- https://prometheus.io/docs/tutorials/alerting_based_on_metrics/ 
- https://webhook.site/
