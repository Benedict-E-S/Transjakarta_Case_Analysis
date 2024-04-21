# modul2_capstone_BES
## Latar Belakang
Transjakarta merupakan sistem Bus yang melayani wilayah Jabodetabek dengan fokus utama di Jakarta Transjakarta beroperasi sejak tahun 2004 dan telah menjadi ikon transportasi publik di ibukota Indonesia. 
Adapun visi misi Transjakarta, yaitu:

Visi: 
- Menjadi perusahaan transportasi berkelas dunia yang menjadi pilihan utama bagi mobilitas masyarakat di DKI Jakarta

Misi:
- Memberikan solusi untuk mengatasi masalah kemacetan dan mobilitas masyarakat di DKI Jakarta
- Menjadi Perusahaan transportasi publik berkelas dunia yang sehat dan berkontribusi positif bagi pemegang saham dan pemangku kepentingan
- Membangun insan yang profesional, peduli dan penuh integritas dengan semangat pelayanan dan gotong royong yang kuat
- menerapkan budaya kerja yang menutamakan pelayanan dan kepuasan pelanggan

## Stakeholder
- Fadly Hasan sebagai Direktur Pelayanan dan Bisnis
- Tim Pelayanan dan Bisnis
## Batasan Data
Dataset dapat diakses [di sini](https://www.kaggle.com/datasets/dikisahkan/transjakarta-transportation-transaction) 
- Dataset ini merupakan data dummy bedasarkan data asli yang didapatkan [di sini](https://ppid.transjakarta.co.id/pusat-data/data-terbuka/transjakarta-gtfs-feed) dengan pengisian baris menggunakan python [Faker](https://faker.readthedocs.io/en/master/) dan [Random](https://docs.python.org/3/library/random.html) 
- Dataset ini hanya mencakup April 2023
- Dataset ini tidak memperhitungkan adanya hari-raya atau cuti bersama.

## Rumusan Masalah:
- Bagaimana tren jumlah transaksi pada April 2023
- Apa yang dapat diketahui tentang pelanggan Transjakarta

## Tujuan masalah:
- Untuk mengetahui kebiasaan transaksi pelanggan Transjakarta dilihat dari transaksi pada April 2023
- Untuk mengetahui demografi pelanggan Transjakarta dilihat dari transaksi pada April 2023
- Untuk memberikan Rekomendasi kepada Stakeholder dalam pengembangan Transjakarta

## Deskripsi Tabel
| No. | Kolom | Deskripsi | 
|-|-|-|
| 1. | **transID** | id unik untuk setiap transaksi | 
| 2. | **payCardID** | id kartu pembayaran pelanggan gunakan sebagai tiket masuk dan keluar bis. Digunakan sebagai pengidentifikasi utama pelanggan | 
| 3. | **payCardBank** | bank penerbit kartu pembayaran pelanggan | 
| 4. | **payCardName** | nama pelanggan pada kartu | 
| 5. | **payCardSex** | jenis kelamin pelanggan pada kartu | 
| 6. | **payCardBirthDate** | tahun lahir pelanggan pada kartu |
| 7. | **corridorID** |  ID koridor/ID rute sebagai kunci untuk pengelompokan |
| 8. | **corridorName** | nama koridor/rute yang mengandung halte awal dan akhir untuk setiap rute | 
| 9. | **direction** | 0 untuk Go, 1 untuk Back. Menentukan arah rute |
| 10. | **apInStops** | ID halte untuk mengidentifikasi halte dimana pelanggan masuk |
| 11. | **tapInStopsName** | nama halte untuk mengidentifikasi halte dimana pelanggan masuk |
| 12. | **tapInStopsLat** | garis bujur halte masuk |
| 13. | **tapInStopsLon** | garis lintang halte masuk |
| 14. | **stopStartSeq** | urutan halte, 1st stop (halte pertama), 2nd stop (halte kedua), dst. Berkaitan dengan arah |
| 15. | **tapInTime** | tanggal dan waktu masuk |
| 16. | **tapOutStops** | ID halte untuk mengidentifikasi halte dimana pelanggan keluar |
| 17. | **tapOutStopsName** | nama halte untuk mengidentifikasi halte dimana pelanggan keluar |
| 18. | **tapOutStopsLat** | garis bujur halte keluar |
| 19. | **tapOutStopsLon** | garis lintang halte keluar |
| 20. | **stopEndSeq** | urutan halte, 1st stop (halte pertama), 2nd stop (halte kedua), dst. Berkaitan dengan arah |
| 21. | **tapOutTime** | tanggal dan waktu keluar |
| 22. | **payAmount** | biaya yang dibayar pelanggan |
