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

### Untuk Tambah/Ubah (Menambahkan Data)
Pada saat nilai/value variable itu 'T'
###
    if pick == 'T' or pick == 't':
       Data[input("Masukkan Nama anda : ")] = [
           input("Masukkan NIM Anda : "),
           int(input("Masukkan Nilai Tugas Anda : ")),
           int(input("Masukkan Nilai UTS Anda : ")),
           int(input("Masukkan Nilai UAS Anda : "))
       ]
Buatlah 'Dictionary' Variable tetapi terisi function input untuk mengisi Data mahasiswa dari User
### Untuk Hapus (Menghapus Data)
Pada saat nilai/value variable itu 'H'
###
    elif pick == 'H' or pick == 'h':
        for ha in range(len(Data)):
            print(ha + 1 ,list(Data.keys())[ha])
        del Data[input("Ketik Nama diatas yang ingin dihapus : ")]
Gunakan for loop untuk menampilkan data yang diisi, kemudian gunakan del untuk menghapus salah satu data tersebut.

### Untuk Lihat (Menampilkan data)
Pada saat nilai/value variable itu 'L'
###
    elif pick == 'L' or pick == 'l':
        print("===========================================")
        print("No |    NIM    |  Nama  | Tugas | UTS | UAS | AKHIR")
        for la in range(len(Data)):
            print(la + 1, ' |',Data[list(Data.keys())[la]][0], '|',list(Data.keys())[la], '|',
                  Data[list(Data.keys())[la]][1], '|' ,
                  Data[list(Data.keys())[la]][2], '|' ,
                  Data[list(Data.keys())[la]][3], '|',
                  Data[list(Data.keys())[la]][1] * 0.3 + Data[list(Data.keys())[la]][2] * 0.35 +
                  Data[list(Data.keys())[la]][3] * 0.35)
        print("===========================================")
Gunakan for loop untuk menampilkan semua Data (Data mahasiswa)

### Untuk Cari (Mencari Data)
Pada saat nilai/value variable itu 'C'
###
    elif pick == 'C' or pick == 'c':
        Find = input("Ketik Nama yang ingin Anda cari : ")
        if Find in list(Data.keys()):
            print('===',Find,'===')
            print('NIM : ',Data[Find][0])
            print('TUGAS : ',Data[Find][1])
            print('UTS : ', Data[Find][2])
            print('UAS : ', Data[Find][3])
        else:
            print("ID Tidak Ditemukan")
Buatlah Variable input dan Gunakan If else Statement. Pada saat variable input itu diketik, data itu akan otomatis menampilkan data yang diinginkan yang sudah diketik

### Untuk Keluar (Keluar dari program / execute)
Pada saat nilai/value variable itu 'K'
###
    elif pick == 'K' or pick == 'k':
        break
Tahap ini akan menutup while loop
![image](https://user-images.githubusercontent.com/61907877/144780789-0cc73620-03bd-48f3-a7ab-2fafb9f9caf8.png)
![image](https://user-images.githubusercontent.com/61907877/144780880-3c514b51-03ce-452a-9864-e1a3fc27d181.png)
![image](https://user-images.githubusercontent.com/61907877/144780940-679f7fb9-c5cb-49f1-a152-6c8d24761678.png)

![Flowchart (1)](https://user-images.githubusercontent.com/61907877/144780991-5058be74-f162-4e31-8365-f6b53c1ab586.png)

