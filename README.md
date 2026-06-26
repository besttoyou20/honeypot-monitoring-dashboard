# Honeypot Monitoring Dashboard with Cowrie, Promtail, Loki, and Grafana

## Deskripsi Proyek
Proyek ini mengimplementasikan sistem monitoring keamanan menggunakan SSH/Telnet Honeypot (**Cowrie**). Log serangan yang dihasilkan oleh Cowrie ditangkap secara *real-time* oleh **Promtail**, kemudian dikirim dan diindeks ke **Grafana Loki**, dan divisualisasikan menggunakan **Grafana Dashboard** untuk analisis aktivitas penyerang.

## Arsitektur Sistem
[Cowrie Logs] ──> [Promtail] ──> [Grafana Loki] ──> [Grafana Dashboard]

## Teknologi yang Digunakan
- **Honeypot:** Cowrie
- **Log Shipper:** Promtail
- **Log Aggregator:** Grafana Loki
- **Visualization:** Grafana

## Struktur Folder
- `configs/`: Berisi seluruh konfigurasi sistem (`cowrie.cfg`, `promtail-config.yaml`, `loki-config.yaml`).
- `grafana/`: Berisi file ekspor dashboard `.json` yang siap di-import kembali.
- `docs/`: Berisi dokumentasi visual sistem dan dashboard.

## Tampilan Dashboard
<p align="center">
  <img src="docs/dashboard/Dashboard1.png" width="30%" alt="Dashboard Log dan IP Overview" />
   <img src="docs/dashboard/Dashboard2.png" width="30%" alt="Dashboard Usename dan Total Event Overview" />
   <img src="docs/dashboard/Dashboard3.png" width="30%" alt="Dashboard Aktivitas Attacker Overview" />
</p>
