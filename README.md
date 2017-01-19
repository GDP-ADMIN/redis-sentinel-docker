# Redis Replication with Sentinel

This is demonstration to show cluster redis in Docker container.
The following docker-compose.yml will create 4 containers as follow
- Redis Node 1 + Sentinel 1
- Redis Node 2 + Sentinel 2
- Sentinel 3
- Sentinel 4
We can simulate redis automatic failover using sentinel.
To launch all containers, run `docker-compose up -d`
