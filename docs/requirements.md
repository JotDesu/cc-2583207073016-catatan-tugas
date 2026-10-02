# Requirements

## Problem Statement
Mahasiswa mengalami kesulitan memantau tenggat tugas dari berbagai
mata kuliah karena informasi tersebar di banyak tempat.

Sistem menyediakan pencatatan tugas, mata kuliah, dan status
pengerjaan sehingga tenggat dapat dipantau dari satu tempat.

## Target Users
- Mahasiswa yang mengambil banyak mata kuliah dengan tugas berbeda-beda

## Functional Requirements
- FR-01 Sistem menampilkan halaman utama.
- FR-02 Sistem menyediakan health endpoint.
- FR-03 Sistem menampilkan metadata aplikasi.
- FR-04 Sistem menampilkan daftar tugas dan mata kuliah (M05 dan seterusnya).

## Non-Functional Requirements
- NFR-01 backend loopback-only
- NFR-02 application managed by systemd
- NFR-03 public request through reverse proxy
- NFR-04 no secret in repository

## Constraints
- 1 vCPU
- 1 GB RAM
- 20 GB disk
- Ubuntu Server 24.04
- public IPv4

## Acceptance Criteria M03
- [x] first deployment accessible
- [x] health endpoint works
