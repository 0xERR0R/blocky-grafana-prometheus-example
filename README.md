# Example: blocky with prometheus and grafana

## How to run

- Clone this repo and execute `docker-compose up`

- Execute some dns queries with `dig @localhost google.com` on linux or `nslookup -q=a google.com 8.8.8.8` on windows. Try to use different domains.

- Open Grafana (see link bellow)

- Click on (+) and import new dashboard

- Paste JSON from https://raw.githubusercontent.com/0xERR0R/blocky/master/docs/blocky-grafana.json

- Select "Prometheus" as data source

- Enter 'http://localhost:4000' as Blocky API Url

- You are done, now you can open the blocky dashboard in Grafana.

## Links

[Prometheus](http://localhost:9090/)

[Grafana](http://localhost:3000/) (use admin/admin as user)

[blocky prometheus endpoint](http://localhost:4000/metrics)