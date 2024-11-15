# labpy4

# Praktikum

    # Inisialisasi list untuk menyimpan data
    data_mahasiswa = []

    while True:
    # Input data mahasiswa
    nama = input("Masukkan Nama mahasiswa: ")
    tugas = float(input("Masukkan Nilai tugas: "))
    uts = float(input("Masukkan Nilai UTS: "))
    uas = float(input("Masukkan Nilai UAS: "))
    
    # Hitung nilai akhir
    nilai_akhir = (tugas * 0.3) + (uts * 0.35) + (uas * 0.35)
    
    # Simpan data ke dalam list
    data_mahasiswa.append({
        'nama': nama,
        'tugas': tugas,
        'uts': uts,
        'uas': uas,
        'nilai_akhir': nilai_akhir
    })
    
    # Tanyakan apakah ingin menambah data
    tambah_data = input("Apakah ada data yang ingin ditambahkan? (y/t): ")
    if tambah_data.lower() == 't':
        break

    # Tampilkan daftar data
    print("\nDaftar Data Mahasiswa:")
    for mahasiswa in data_mahasiswa:
    print(f"Nama: {mahasiswa['nama']}, Tugas: {mahasiswa['tugas']}, UTS: {mahasiswa['uts']}, UAS: {mahasiswa['uas']}, Nilai Akhir: {mahasiswa['nilai_akhir']:.2f}")
PENJELASAN 
1.	Penggunaan while True berguna untuk terus meminta input dari pengguna atau pengulangan sampai diputuskan untuk berhenti oleh sang pengguna dengan menjawab antara 'y' atau 't'
2.	Penginputan data mahasiswa yang berisi nama, nilai tugas, UTS, UAS, bertipe float yang memungkinkan pengguna memasukkan angka desimal
3.	Penghitungan nilai akhir berdasarkan bobot yang telah ditentukan seperti, tugas:30%, UTS35%, UAS35% dan hasil penghitungan nilai akhir disimpan kedalam variable nilai_akhir
4.	Penyimpanan data kedalam list dengan menggunakan metode append()
5.	Menanyakan apakah ada data yang ingin ditambahkan atau tidak. Jika jawabannya 't' maka program akan berhenti dan mengeluarkan hasil penghitungan
6.	Menampilkan data yang telah selesai diolah

![Screenshot 2024-11-15 102947](https://github.com/user-attachments/assets/78e3477f-d1da-4bff-8b7a-591a152bf559)

# Latihan

    # Membuat list dengan 5 elemen
    A = [10, 20, 30, 40, 50]

    # Akses list
    print("List A:", A)

    # Tampilkan elemen ke-3
    print("Elemen ke-3:", A[2])

    # Ambil nilai elemen ke-2 sampai elemen ke-4
    print("Elemen ke-2 sampai ke-4:", A[1:4])

    # Ambil elemen terakhir
    print("Elemen terakhir:", A[-1])

    # Ubah elemen list
    # Ubah elemen ke-4 dengan nilai lainnya
    A[3] = 100
    print("Setelah mengubah elemen ke-4:", A)

    # Ubah elemen ke-4 sampai dengan elemen terakhir
    A[3:] = [200, 300]
    print("Setelah mengubah elemen ke-4 sampai terakhir:", A)

    # Tambah elemen list
    # Ambil 2 bagian dari list pertama (A) dan jadikan list ke-2 (B)
    B = A[1:3]
    print("List B (dari A):", B)

    # Tambah list B dengan nilai string
    B.append("String")
    print("Setelah menambah string ke B:", B)

    # Tambah list B dengan 3 nilai
    B.extend([400, 500, 600])
    print("Setelah menambah 3 nilai ke B:", B)

    # Gabungkan list B dengan list A
    C = A + B
    print("List C (gabungan A dan B):", C)
PENJELASAN
1. Mengakses elemen ke-3 dari list A. Dalam Python, indeks dimulai dari 0, jadi A[2] merujuk pada elemen ketiga, yaitu 30.
2. Mengambil elemen dari indeks 1 sampai 3 (indeks 4 tidak termasuk). Ini akan menghasilkan list baru yang berisi [20, 30, 40].
3. Mengakses elemen terakhir dari list A menggunakan indeks negatif. A[-1] merujuk pada elemen terakhir, yaitu 50.
4. Mengubah elemen ke-4 (indeks 3) menjadi 100. Setelah perubahan, list A menjadi [10, 20, 30, 100, 50].
5. Mengubah elemen dari indeks 3 hingga akhir list menjadi [200, 300]. List A sekarang menjadi [10, 20, 30, 200, 300].

![Screenshot 2024-11-15 103549](https://github.com/user-attachments/assets/41b9a71b-bbbd-4d1c-83cf-3a97d1f9ce03)

![flowchartt](https://github.com/user-attachments/assets/772301f0-45a4-4950-b40f-38220c397097)

