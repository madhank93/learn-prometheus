### Prometheus architecture

![prometheus-architecture](docs/img/prom_architecture.png)

#### Prometheus server

- **Retrieval** - Pulls metrics data from target services like applications, servers and services ...etc
- **Storage** - Stores scraped metrics in a Time series DB
- **HTTP server** - web server displays data in an UI (prometheus web ui) which accepts PromQL query language

### Levels of Monitoring

- Infrastructure level - CPU, RAM, Network ... etc
- Platform level - Kubernetes components, Docker, Bare server
- Application level - 3rd party application and Our own applications

### What does it monitor ?

- CPU status
- Memory/Disk usage
- API requests count
- Exception count

### Type of metrics

- **Counter** - How many times this event happened ? (ex: no. of exception, total no. of request a service as received)
- **Gauge** - What is the current value of this event now ? Values can go up and down (ex: current usage of RAM or DISK)
- **Histogram** - It is used to track how long an event took ? (eg: how long an API request took to complete)
