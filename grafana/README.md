# Prometheus config

## Gathering info

Edit the `prometheus.yml` file to add extra nodes/containers to scrape data from:

- X = name
- Y = target
- Z = port

```
  - job_name: "X"
    static_configs:
      - targets: ["Y:Z"]
```
