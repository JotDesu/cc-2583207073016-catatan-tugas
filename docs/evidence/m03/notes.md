# Evidence M03

- Tanggal: 2 Oktober 2026
- Gunicorn hanya di 127.0.0.1:8000 (lihat ports.txt)
- UFW: OpenSSH dan 80/tcp ALLOW (lihat ufw.txt)
- Health internal (:8000) dan lewat Caddy (:80) mengembalikan status ok
- Health eksternal dari Windows: HTTP 200 via Caddy (health-external.txt)
- Screenshot browser: (tambahkan jika ada)
- Screenshot browser (Chrome, Windows): browser-home.png dan browser-health.png
