# cc-25832071008-eduquizstudio

Cloud Computing — PTI 2802  
Pertemuan 3 — Project Inception

## Author
- **Nama:** [Neira Puja Fazriani]
- **NIM:** [25832071008]
- **Kelas:** [2A]

## Problem
Deployment aplikasi web Flask ke infrastruktur VPS Ubuntu Server 24.04 menggunakan Gunicorn, systemd, dan reverse proxy Caddy.

## Target Users
Mahasiswa dan Dosen Pengampu Mata Kuliah Cloud Computing (PTI 2802).

## Features M03
- baseline application (`/`)
- health check endpoint (`/health`)
- VPS deployment dengan Caddy & systemd

## Architecture

```mermaid
flowchart LR
    U[User] --> C[Caddy]
    C --> G[Gunicorn]
    G --> F[Flask]
