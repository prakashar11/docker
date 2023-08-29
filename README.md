# OpenCTI Docker deployment

## Setting up considerations

1. .env file to be populated with necessary tokens
2. Network to be incuded in docker compose file that starts platform/workers
```
docker network ls
```
3. Update relevant connector docker compose files with necessary details e.g., ADMIN_TOKEN to be used by the connectors to connect to platform/workers and also data source URL to be configured
4. To start relevant connector separately
```
docker-compose -f mitre-docker-compose.yml up -d
docker-compose -f cisa-docker-compose.yml up -d
```
5. To restart only a specific container that needs to be recreated/restarted
```
docker-compose restart <container name in docker compose.yml>
```

## Documentation

You can find the detailed documentation about the Docker installation in the [OpenCTI documentation space](https://docs.opencti.io/latest/deployment/installation/#using-docker).

## Community

### Status & bugs

Currently OpenCTI is under heavy development, if you wish to report bugs or ask for new features, you can directly use the [Github issues module](https://github.com/OpenCTI-Platform/opencti/issues).

### Discussion

If you need support or you wish to engage a discussion about the OpenCTI platform, feel free to join us on our [Slack channel](https://community.filigran.io). You can also send us an email to contact@opencti.io.

## About

### Authors

OpenCTI is a product designed and developed by the company [Filigran](https://www.filigran.io).

<a href="https://www.filigran.io" alt="Filigran"><img src="https://www.filigran.io/wp-content/uploads/2022/08/filigran_text_horizontal_dense_margin.png" width="230" /></a>
