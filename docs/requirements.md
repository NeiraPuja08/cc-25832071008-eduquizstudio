# Requirements

## Problem Statement
Deployment aplikasi Flask pada infrastruktur VPS Ubuntu Server 24.04 dengan reverse proxy Caddy dan manajemen service menggunakan systemd.

## Target Users
Mahasiswa dan Dosen Pengampu Matakuliah Cloud Computing (PTI 2802).

## Functional Requirements
- FR-01 Aplikasi menyajikan halaman utama pada endpoint `/`.
- FR-02 Aplikasi menyediakan health check pada endpoint `/health`.
- FR-03 Aplikasi menyediakan informasi metadata pada endpoint `/api/info`.

## Non-Functional Requirements
- NFR-01 backend loopback-only (127.0.0.1:8000).
- NFR-02 application managed by systemd.
- NFR-03 public request through reverse proxy (Caddy port 80).
- NFR-04 no secret in repository.

## Constraints
- 1 vCPU
- 1 GB RAM
- 20 GB disk
- Ubuntu Server 24.04
- public IPv4

## Acceptance Criteria M03
- [x] first deployment accessible
- [x] health endpoint works
