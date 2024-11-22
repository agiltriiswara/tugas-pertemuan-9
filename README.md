NAMA : AGIL TRI ISWARA
KELAS: IE.23.C12
NIM  : 352310848

# Program untuk menambahkan data ke dalam list

# List untuk menyimpan data mahasiswa
data_mahasiswa = []

while True:
    # Memasukkan data mahasiswa
    nama = input("Nama: ")
    nim = input("NIM: ")
    nilai_tugas = float(input("Nilai Tugas: "))
    nilai_uts = float(input("Nilai UTS: "))
    nilai_uas = float(input("Nilai UAS: "))
    
    # Menghitung nilai akhir
    nilai_akhir = (nilai_tugas * 0.3) + (nilai_uts * 0.35) + (nilai_uas * 0.35)
    
    # Menambahkan data ke dalam list
    data_mahasiswa.append({
        "Nama": nama,
        "NIM": nim,
        "Tugas": nilai_tugas,
        "UTS": nilai_uts,
        "UAS": nilai_uas,
        "Akhir": nilai_akhir
    })
    
    # Menanyakan apakah ingin menambahkan data lagi
    tambah_data = input("Tambah data (y/t)? ").lower()
    if tambah_data == 't':
        break

# Menampilkan data
print("\n{:<5} {:<15} {:<10} {:<10} {:<10} {:<10} {:<10}".format(
    "No", "Nama", "NIM", "Tugas", "UTS", "UAS", "Akhir"))
print("=" * 65)

for i, mahasiswa in enumerate(data_mahasiswa, start=1):
    print("{:<5} {:<15} {:<10} {:<10} {:<10} {:<10} {:<10.2f}".format(
        i, mahasiswa["Nama"], mahasiswa["NIM"], mahasiswa["Tugas"],
        mahasiswa["UTS"], mahasiswa["UAS"], mahasiswa["Akhir"]))



<img width="960" alt="visual code" src="https://github.com/user-attachments/assets/9175ac14-6928-4d57-818c-b67a81950fe3">













PENJELASAN PROGRAM

List data_nilai: Digunakan untuk menyimpan data yang dimasukkan, termasuk nilai tugas, UTS, UAS, dan nilai akhir.
Perulangan while True: Perulangan yang terus berlangsung selama pengguna memilih untuk menambah data (menjawab "y").
Input Nilai: Program meminta input nilai tugas, UTS, dan UAS, kemudian menghitung nilai akhir berdasarkan bobot yang diberikan.
Menyimpan Data: Data dimasukkan ke dalam list data_nilai, di mana setiap elemen berupa list yang berisi nilai tugas, UTS, UAS, dan nilai akhir.
Pertanyaan untuk Menambah Data: Setelah memasukkan data, program akan menanyakan apakah ingin menambah data lagi dengan menjawab "y" (ya) atau "t" (tidak).
Menampilkan Daftar Nilai: Jika pengguna memilih untuk tidak menambah data, program akan menampilkan seluruh data yang telah dimasukkan dengan format yang rapi






FLOW CHART

![Picture1](https://github.com/user-attachments/assets/22be339a-3114-4049-b4db-c29e39d39db6)


    
