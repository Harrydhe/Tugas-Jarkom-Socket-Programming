# Tugas1-Socket-Programming

# Analisis TCP pada Simple Socket Programming

Tutorial ini menjelaskan bagaimana TCP bekerja pada Socket Programming dengan bantuan **Wireshark**. Dalam tutorial ini, Anda akan membuat program socket sederhana dan menggunakan Wireshark untuk menganalisis paket TCP yang dikirimkan selama komunikasi antara client dan server.

## Persiapan Program Socket

Ikuti langkah-langkah berikut untuk mempersiapkan program socket:

1. **Buka direktori Program Socket**
   - Masuk ke direktori `/simple-socket-programming`:
     ```bash
     cd /simple-socket-programming
     ```

2. **Sesuaikan Port Number di File Server**
   - Buka file `server.c` dan sesuaikan port number pada baris ke-40:
     ```c
     const uint16_t port_number = 50000;
     ```
   - Pastikan port number yang digunakan adalah `50000`.

3. **Sesuaikan Port Number di File Client**
   - Buka file `client.c` dan sesuaikan nilai port number pada baris ke-19:
     ```c
     portno = 50000;
     ```
   - Pastikan nilai port number di file client sama dengan file server.

## Menjalankan Program Socket

1. **Buka Terminal**
   - Buka terminal pada aplikasi Anda.

2. **Masuk ke Direktori Program**
   - Arahkan terminal ke direktori tempat program berada:
     ```bash
     cd {path_to_root_dir}/tugas-1/simple-socket-programming
     ```

3. **Kompilasi Program**
   - Jalankan perintah `make` untuk mengompilasi program:
     ```bash
     make
     ```

4. **Jalankan Aplikasi Wireshark**
   - Untuk menganalisis lalu lintas jaringan menggunakan Wireshark, jalankan Wireshark dengan perintah:
     ```bash
     sudo wireshark
     ```

5. **Pilih Loopback Interface**
   - Di Wireshark, pilih interface **Loopback: lo0** untuk menangkap paket yang dikirim melalui jaringan lokal.
   ![Diagram Socket](aset/picture1.png)

