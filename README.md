
# TIG Stack untuk MDT
> TIG = Telegraf, InfluxDB, dan Grafana\
> MDT = Model Driven Telemetry

###### Desclaimer
This repo's guide is written in Bahasa Indonesia. This repo is intended as learning purpose or trial.\
Petunjuk repo ini ditulis dalam Bahasa Indonesia. Repo ini ditujukan untuk tujuan pembelajaran atau percobaan.

## Daftar Cek Pekerjaan
- [x] Mekanisme Dial Out
- [ ] Mekanisme Dial In

## Presentasi Tentang Telemetry
- https://www.youtube.com/watch?v=9ZE8qPkfqxE
- https://www.youtube.com/watch?v=tIN8BjHwpNs

## Sandbox atau LAB
- [Model Driven Telemetry Devnet Sandbox](https://devnetsandbox.cisco.com/RM/Diagram/Index/0e053963-b039-4a15-94f6-54db2f5ad61c?diagramType=Topology)

## Cara Mencoba
1. Pastikan bahwa Docker dan Docker-Compose sudah terinstall.\
[Cara Install Docker](https://docs.docker.com/get-docker/) dan [Cara Install Docker-Compose](https://docs.docker.com/compose/install/)
2. Clone repo ini
     ```
      $ git clone https://github.com/haidlir/TIG-Stack-Streaming-Telemetry.git
    ```
3. Hidupkan dengan mengeksekusi file up.sh
   ```
    $ ./up.sh
   ```
4. Buka Grafana di http://localhost:3000
5. Buat data source ke InfluxDB\
Username dan Pasword dapat dilihat di file ```.env```
6. Import Dashboard dari file ```fixtures/grafana-mdt.json```
7. Konfigurasi Router Cisco (IOS-XR) seperti yang ada di ```fixtures/IOS-XR-Configuration.cfg```

### Cuplikan Gambar
![Grafana-MDT](https://raw.githubusercontent.com/haidlir/TIG-Stack-Streaming-Telemetry/master/img/grafana-mdt.png "Grafana-MDT")

## Credits
1. InfluxData
2. Grafana Labs
3. Cisco DevNet

###### Notes
Bila butuh bantuan dalam mengimplementasikan hal serupa di lingkungan produksi atau operasional, kami terbuka untuk berkolaborasi. [Kontak kami](http://www.netmonk.id)
