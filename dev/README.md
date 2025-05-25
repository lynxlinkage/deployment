# Development Environment

This directory contains the Docker Compose configuration for the local development environment of LynxLinkage.

## Components

- **PostgreSQL**: Database server
- **Authentik**: Open-source Identity Provider (IdP) for authentication and authorization
- **Redis**: Required for Authentik's operation

## Getting Started

1. Make sure Docker and Docker Compose are installed on your system
2. Update the `.env` file with secure passwords
3. Start the environment:

```bash
docker-compose up -d
```

4. Access the Authentik admin interface at http://localhost:9000
5. For the first-time setup, follow the Authentik setup wizard

## Configuration

- All environment variables are stored in the `.env` file
- Database data is persisted in Docker volumes

## Stopping the Environment

```bash
docker-compose down
```

To completely remove all data (volumes):

```bash
docker-compose down -v
```
