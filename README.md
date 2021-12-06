# Tugas-Praktikum
## Buat program sederhana yang akan menampilkan daftar nilai mahasiswa

### 1 - Buatlah dan gunakan 'Dictionary' variable
    Data = {
      "Raphael" : ['312110173' , 90, 90, 90],
      "Michael" : ['312110174' , 100, 90, 80]
    }
### 2 - Buatlah perulangan (while loop) dan variable - input() untuk menampilkan menu pilihan
    while True:
      pick = input("(T)ambah/ubah, (H)apus, (L)ihat, (C)ari, (K)eluar : ")

### Untuk Tambah
Pada saat nilai/value variable itu 'T'
###
    if pick == 'T' or pick == 't':
       Data[input("Masukkan Nama anda : ")] = [
           input("Masukkan NIM Anda : "),
           int(input("Masukkan Nilai Tugas Anda : ")),
           int(input("Masukkan Nilai UTS Anda : ")),
           int(input("Masukkan Nilai UAS Anda : "))
       ]

