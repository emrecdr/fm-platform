# Api Platform
Api Platform is responsible for ddockerization of gateway and services.
All system elements can be started by running `$ docker-compose up` command.
When you start system it will start:
- Rabbitmq
- Api Gateway: https://github.com/siluet/fm-gateway.git
- Logger (1 for tracking, 1 for error logs): https://github.com/siluet/fm-log.git
- Product Service: https://github.com/siluet/fm-service-product.git
- Basket Service: https://github.com/siluet/fm-service-basket.git

### Installation
1. `$ docker-compose up`  or  `$ docker-compose up -d` will start whole backend systems.

#### Postman
All gateway endpoints can be tested through postman.

#### Logs
After startin system, tracking logs can be viewed by executing `$ docker-compose logs -f logger-trace` on project root.
Error logs (fatal, error, warning) can be viewed by `$ docker-compose logs -f logger-error`.
