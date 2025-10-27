# System Architecture

## Overview
DevOps Simulator follows a microservices architecture for production and a simplified stack for development.

## Components
- *App Server*: Node.js + Express (prod port 8080, dev 3000)
- *Database*: PostgreSQL (prod HA, dev single instance)
- *Monitoring*: Prometheus+Grafana in prod; console logs in dev

## Deployment
- Production: Rolling updates, zero-downtime, region us-east-1
- Development: Docker Compose, hot-reload, local testing

## Security
- Production: SSL/TLS, strict access controls
- Development: Relaxed security for debugging

## Experimental
- Experimental features are documented but disabled by default.