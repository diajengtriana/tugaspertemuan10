# Tugas pertemuan 10
# Nama  : Diajeng triana k.
# Nim   : 312110474
# Kelas : TI.21.C5
# Latihan 1
pada latiahan 1 saya diberi soal sebagai berikut :

<img width="476" alt="soal latihan 1" src="https://user-images.githubusercontent.com/92905452/145263873-97b3634c-d8f3-4614-bf66-1bc57b095538.png">

# Jawab
1. Saya membuat data kontak awal

    b={'ari':'085267888','dina':'087677776'}

2. saya diberi soal untuk menampilkan kontak ari

    print(b['ari'])

3. saya disuruh menambah kontak atas nama riko

    b['riko']='087654544'

4. mengubah kontak dina

    b['dina']='088999776'

5. tampilkan semua nama

    print(b.keys())

6. tampilkan semua nomor

    print(b.values())

7. menampilkan semua nama dan nomor

    print(b)

8. menghapus kontak dina

    del b['dina']

# Output

<img width="627" alt="outputlatihan1" src="https://user-images.githubusercontent.com/92905452/145265149-79ebe1ec-b4ab-4c4f-a75d-a472556b7b45.png">

# Tugas Praktikum
pada tugas praktium saya diberi soal sebagai berikut:

<img width="540" alt="tugas praktikum" src="https://user-images.githubusercontent.com/92905452/145265973-abfa3efd-b343-4bbf-bef2-a334dea7681b.png">


# Flowchart

<img width="345" alt="flowchart" src="https://user-images.githubusercontent.com/92905452/145265546-bf2d8c47-0ad2-4261-a55f-4ca227e14f35.png">

# Jawab
pertama saya membuat looping agar program terus berjalan
while True:
    c = input("\n(L)ihat, (T)ambah, (U)bah, (H)apus, (C)ari, (K)eluar: ")
lalu saya membuat format if untuk memasukan pilihan , sebagai contoh apabila memilih (t) akan menambah data
if (c.lower() == 't'):
        print('\nTambah Data Mahasiswa Baru')
        nama= input("Masukkan Nama\t\t: ")
        nim= input("Masukkan NIM\t\t: ")
        nilaiTugas= int(input("Masukkan Nilai Tugas\t: "))
        nilaiUts= int(input("Masukkan Nilai UTS\t: "))
        nilaiUas= int(input("Masukkan Nilai UAS\t: "))
        nilaiAkhir= (0.30 * nilaiTugas) + (0.35 * nilaiUts) + (0.35 * nilaiUas)
        dataMhs[nama]= nim, nilaiTugas, nilaiUts, nilaiUas, nilaiAkhir
        print("\nData Berhasil Ditambahkan!")
saya juga melakukan percabangan if (elif) untuk melaksanakan pilihan yang lain
elif (c.lower() == 'u'):
        print('\nMengedit Data Mahasiswa')
        nama = input("Masukkan Nama: ")
        if nama in dataMhs.keys():
            nim= input("Masukkan NIM Baru\t: ")
            nilaiTugas= int(input("Masukkan Nilai Tugas\t: "))
            nilaiUts= int(input("Masukkan Nilai UTS\t: "))
            nilaiUas= int(input("Masukkan NIlai UAS\t: "))
            nilaiAkhir= (0.30 * nilaiTugas) + (0.35 * nilaiUts) + (0.35 * nilaiUas)
            dataMhs[nama] = nim, nilaiTugas, nilaiUts, nilaiUas, nilaiAkhir
            print("\nData Berhasil Di Update!")
dan saya juga menggunakan else untuk apabila salah memasukan pilihan inputan
 else:
        print("Pilih menu yang tersedia: ")
# Output
ini adalah output apabila memilih tambah(t)
