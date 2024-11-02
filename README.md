# GitHub Action - Create prometheus scrape config

This GitHub Action helps to create prometheus scrape config


## Usage

Add this step in your workflow file
```yaml
-   name: Create prometheus scrape config
    id: create_prometheus_scrape_config
    uses: A-A-S-DevLab/actions-create-prometheus-scrape-config@v1.0.0
    with:
        directory: ./
        filename: config.yml
        domain_name: test.domain.com
        server_local_ip: 192.168.0.111
        service_port: 8080
```

## Input variables

- `directory`: Target directory
- `filename`: Target file name
- `domain_name`: Service domain name
- `server_local_ip`: Service IP in local network
- `service_port`: Service port in local network