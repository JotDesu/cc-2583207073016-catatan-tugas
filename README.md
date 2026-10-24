# BrewPoint: Aplikasi Kasir Web untuk Kedai Kopi dengan Dashboard Pemilik

Cloud Computing — PTI 2802  
Pertemuan 3 — Project Inception

## Author
Andiana Jamaludin Malik / 2583207073016 / 2 B

## Problem
Pencatatan penjualan kedai kopi kecil masih dilakukan manual sehingga
rekap harian lambat, rawan salah catat, dan pemilik tidak dapat memantau
penjualan dari jarak jauh. (Bukti wawancara menyusul.)

## Target Users
- Barista atau kasir kedai kopi
- Pemilik kedai kopi

## Features M03
- baseline application
- health endpoint
- VPS deployment

## Planned Features
- kasir web: daftar menu, keranjang, simpan transaksi
- dashboard pemilik: laporan harian dan produk terlaris
- kelola menu dan harga, login pemilik

## Architecture

```mermaid
flowchart LR
    U[User] --> C[Caddy]
    C --> G[Gunicorn]
    G --> F[Flask]
```

## Infrastructure
- Microsoft Azure (Azure for Students), East Asia
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
