# Student Task Tracker

Cloud Computing — PTI 2802  
Pertemuan 3 — Project Inception

## Author
(Andiana Jamaludin Malik / 2583207073016 / 2B)

## Problem
Mahasiswa kesulitan memantau tenggat tugas dari berbagai mata kuliah
karena informasi tersebar di banyak tempat.

## Target Users
Mahasiswa yang mengambil banyak mata kuliah dengan tugas berbeda-beda.

## Features M03
- baseline application
- health endpoint
- VPS deployment

## Architecture

```mermaid
flowchart LR
    U[User] --> C[Caddy]
    C --> G[Gunicorn]
    G --> F[Flask]
```

## Infrastructure
- Ubuntu Server 24.04
- 1 vCPU
- 1 GB RAM
- 20 GB disk
- Caddy
- Gunicorn

## Public Endpoint
`http://65.52.163.162/`

## Health Check
`GET /health`

## Deployment
See `docs/deployment.md`.

## Security
- key-only SSH
- root SSH disabled
- UFW enabled
- backend loopback-only

## Current Limitations
- HTTP only
- no persistent database
- no container
- manual deployment

## Roadmap
M04 DNS/HTTPS, M05 Data, M06 Container, M07 IaC, M09 CI/CD
