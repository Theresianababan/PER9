# PER9
<H1>from prettytable import PrettyTable

def hitung_nilai_akhir(tugas, uts, uas):
    nilai_akhir = 0.3 * tugas + 0.35 * uts + 0.35 * uas
    return nilai_akhir

# Inisialisasi list untuk menyimpan data
data_mahasiswa = []

while True:
    # Meminta input data
    nomor_induk = input("Masukkan nomor induk mahasiswa: ")
    nama = input("Masukkan nama mahasiswa: ")
    tugas = float(input("Masukkan nilai tugas: "))
    uts = float(input("Masukkan nilai UTS: "))
    uas = float(input("Masukkan nilai UAS:"))

    # Menghitung nilai akhir
    nilai_akhir = hitung_nilai_akhir(tugas, uts, uas)

    # Menambahkan data ke dalam list
    data_mahasiswa.append({
        'Nomor Induk': nomor_induk,
        'Nama': nama,
        'Tugas': tugas,
        'UTS': uts,
        'UAS': uas,
        'Nilai Akhir': nilai_akhir
    })

    # Menanyakan apakah ingin menambahkan data lagi
    jawaban = input("Tambahkan data lagi? (y/t): ")
    if jawaban.lower() != 'y':
        break

# Membuat tabel menggunakan PrettyTable
tabel = PrettyTable()
tabel.field_names = ["No. Induk", "Nama", "Tugas", "UTS", "UAS", "Nilai Akhir"]

# Menambahkan data ke dalam tabel
for mahasiswa in data_mahasiswa:
    tabel.add_row([
        mahasiswa['Nomor Induk'],
        mahasiswa['Nama'],
        mahasiswa['Tugas'],
        mahasiswa['UTS'],
        mahasiswa['UAS'],
        mahasiswa['Nilai Akhir']
    ])

# Menampilkan tabel
print("\nDaftar Nilai Mahasiswa:")
print(tabel)</H1>
<H1># Buat list dengan 5 elemen
list_a = [10, 20, 30, 40, 50]

# Akses list
# Tampilkan elemen ke 3
print("Elemen ke-3:", list_a[2])

# Ambil nilai elemen ke 2 sampai elemen ke 4
print("Elemen ke-2 sampai ke-4:", list_a[1:4])

# Ambil elemen terakhir
print("Elemen terakhir:", list_a[-1])

# Ubah elemen list
# Ubah elemen ke 4 dengan nilai lainnya
list_a[3] = 45
print("Setelah mengubah elemen ke-4:", list_a)

# Ubah elemen ke 4 sampai dengan elemen terakhir
list_a[3:] = [50, 60, 70]
print("Setelah mengubah elemen ke-4 sampai terakhir:", list_a)

# Tambah elemen list
# Ambil 2 bagian dari list pertama (A) dan jadikan list ke 2 (B)
list_b = list_a[:2]
print("List B:", list_b)

# Tambah list B dengan nilai string
list_b.append("Hello")
print("List B setelah tambah string:", list_b)

# Tambah list B dengan 3 nilai
list_b.extend([1, 2, 3])
print("List B setelah tambah 3 nilai:", list_b)

# Gabungkan list B dengan list A
list_c = list_a + list_b
print("List setelah menggabungkan list A dan B:", list_c)</H1>

![2c643da7-a6de-43f5-acdc-087862d88cdd](https://github.com/Theresianababan/PER9/assets/148035194/dc319bab-b7af-4fff-a87c-6fb043d8838d)


![2c643da7-a6de-43f5-acdc-087862d88cdd](https://github.com/Theresianababan/PER9/assets/148035194/020cf181-90a0-4197-a5e8-28797fe46870)




![ss39](https://github.com/Theresianababan/PER9/assets/148035194/00253fc1-eacf-4fa6-8860-ef74fd604f3b)
