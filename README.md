# PjBL Jaringan Komputer: Smart Hospital Network

Repositori ini berisi dokumentasi, laporan progres, dan file simulasi proyek untuk mata kuliah Jaringan Komputer dan Komunikasi Data.

## Deskripsi Proyek
Proyek ini merancang arsitektur infrastruktur jaringan **Smart Hospital** menggunakan simulasi GNS3. Jaringan dirancang menggunakan metode segmentasi *Virtual Local Area Network* (VLAN), *Inter-VLAN Routing* dengan model *Router-on-a-Stick*, serta alokasi IP Address yang efisien menggunakan metode perhitungan VLSM (*Variable Length Subnet Mask*).

## Anggota Tim
* Farrel Razan Aryaputra (GitHub: @LazYenggg)
* Misye Khalina Aprilia Marbun (GitHub: @misyekhalinaapriliamarbun)

## Status Pengerjaan (Progres)
* [x] **Progres 1:** Proposal Analisis Kebutuhan, Subnetting VLSM, dan Desain Topologi (Selesai).
* [x] **Progres 2:** Implementasi VLAN dan Pemetaan Port Akses pada Switch (Selesai).
* [x] **Progres 3:** Konfigurasi Trunking, Inter-VLAN Routing, dan Pengujian Konektivitas (Selesai).
* [ ] **Final:** Implementasi Layanan Server (Ubuntu), Analisis Lanjutan, Laporan Akhir, dan Presentasi.

## Catatan Teknis (Progres 3)
Pada tahapan simulasi Progres 3, *node* layanan server (Ubuntu Web Server & Database Server) pada area VLAN 40 disimulasikan menggunakan Virtual PC Simulator (VPCS) sebagai penyesuaian (*workaround*) atas limitasi akselerasi perangkat keras/virtualisasi (KVM) pada mesin *host*. 

Meskipun menggunakan simulator yang lebih ringan, pengujian fungsionalitas lintas VLAN (melalui metode *Ping* dan *Traceroute*) serta logika *routing* menggunakan metode *Router-on-a-Stick* telah tervalidasi dan beroperasi 100% secara fungsional sesuai dengan IP Plan. Instalasi sistem operasi Linux (*Ubuntu Server*) definitif ditargetkan pada Tahap Final.

## Struktur File
* `Proposal Project Akhir Jaringan Komputer Kelompok 1.pdf` : Laporan lengkap Progres 1 berisi latar belakang, tabel VLSM, dan diagram arsitektur jaringan.
* `Proposal Project Akhir Jaringan Komputer Kelompok 1_Progress 2.pdf` : Laporan untuk Progres 2 berisi konfigurasi dan implementasi database VLAN.
* `Laporan Project Akhir Jaringan Komputer Kelompok 1_Progress3.pdf` : Laporan kelanjutan untuk Progres 3 berisi konfigurasi Inter-VLAN Routing dan hasil pengujian konektivitas lintas divisi.
* `Screenshot_Progress2/` : Folder berisi bukti *screenshot* konfigurasi VLAN pada GNS3.
* `Screenshot_Progress3/` : Folder berisi bukti *screenshot* konfigurasi antarmuka *Trunk*, *Sub-Interface* Router, dan verifikasi tabel rute.
* `Smart_Hospital_Prog2.zip` : File arsip (*export*) proyek simulasi GNS3 untuk tahapan Progres 2.
* `Smart_Hospital_Prog3.zip` : File arsip (*export*) proyek simulasi GNS3 terbaru untuk tahapan Progres 3.
* `Video Demonstrasi pada Progress 2.mkv` : Rekaman layar yang menunjukkan hasil verifikasi tabel VLAN.
* `Video Demonstrasi Progress 3.mkv` : Rekaman layar demonstrasi *ping*, *traceroute*, dan *routing table* (Progres 3).
