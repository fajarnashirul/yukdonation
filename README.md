# yukdonation - Donation Platform

Microservices-based donation platform for Zakat, Sadaqah, Waqf, Qurbani, and General donations.

## Architecture

## Services

| Service | Description | Repo                                                                      |
|---------|-------------|---------------------------------------------------------------------------|
| Config Server | Centralized configuration | [link](https://github.com/fajarnashirul/yukdonation-config-server.git)    |
| API Gateway | Auth (JWT), routing, rate limiting | [link](https://github.com/fajarnashirul/yukdonation-api-gateway.git)      |
| Donation Service | Campaigns, donations, saga, business rules | [link](https://github.com/fajarnashirul/yukdonation-donation-service.git) |
| Payment Service | Midtrans integration, webhooks | [link](https://github.com/fajarnashirul/yukdonation-payment-service.git)  |

## Quick Start

```bash
git clone --recurse-submodules https://github.com/fajarnashirul/yukdonation.git
cd yukdonation
cp .env.example .env  # Add your Midtrans keys and database config
docker-compose up --build -d
```
