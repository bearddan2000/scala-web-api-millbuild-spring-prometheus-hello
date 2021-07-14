# scala-web-api-millbuild-spring-prometheus-hello

## Description
Another way to serve web content.
Uses prometheus to track visitors
and grafana to visualize low level
metrics.

To see a graph of visitors:
- Nav to http://localhost:81
- Classic UI
  - Click Graph tab
    - Search: 'scrape_series_added'
      or 'scrape_duration_second'
      or 'http_request_duration_ms_bucket'
    - Duration 1m

For health check:
- Nav to http://localhost:81
- Targetes

## Tech stack
- scala
- millbuild
- prometheus

## Docker stack
- nightscape/scala-mill
- prom/prometheus:latest

## To run
`sudo ./install.sh -u`
- Available http://localhost
- App metrics http://localhost/metrics
- Prometheus console http://localhost:81

## To stop
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`

## Credit
- https://github.com/monodot/spring-boot-with-metrics/blob/main/pom.xml
