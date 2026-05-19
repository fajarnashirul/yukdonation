# yukdonation - Donation Platform

Microservices-based donation platform for Zakat, Sadaqah, Waqf, Qurbani, and General donations.

## Architecture

## Services

| Service | Description | Repo |
|---------|-------------|------|
| Config Server | Centralized configuration | [link] |
| API Gateway | Auth (JWT), routing, rate limiting | [link] |
| Donation Service | Campaigns, donations, saga, business rules | [link] |
| Payment Service | Midtrans integration, webhooks | [link] |

## Quick Start

```bash
git clone --recurse-submodules https://github.com/fajarnashirul/yukdonation.git
cd yukdonation
cp .env.example .env  # Add your Midtrans keys
docker-compose up --build -d
```
