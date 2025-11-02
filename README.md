# **Tugas Praktikum 4 – labpy03**

# *Latihan 1 - Bilangan Acak Kurang dari 0.5*

n = int(input("Masukkan nilai N: "))

i = 0
while i < n:
    a = random()  # menghasilkan angka acak antara 0 dan 1
    if a < 0.5:   # hanya tampilkan jika < 0.5
        print(f"data ke: {i+1} => {a}")
        i += 1

print("Selesai")

Alur Algoritma
1. Import fungsi random() dari modul random.
2. Program meminta input jumlah data N.
3. Menggunakan perulangan while untuk menampilkan data acak.
4. Hanya bilangan dengan nilai kurang dari 0.5 yang ditampilkan.
5. Program berhenti setelah menampilkan N data.

Hasil Screenshot
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/6da5d6e7-ed1c-4a98-9328-2193dd961c0e" />

# *Latihan 2 – Menghitung Laba Usaha*

Kode Program (latihan2.py)

# Modal awal
modal = 100000000

# Inisialisasi total laba
total = 0

# Perulangan selama 8 bulan
for i in range(1, 9):
    if i == 1 or i == 2:
        laba = 0
    elif i == 3 or i == 4:
        laba = modal * 0.1   # 10% dari modal
    elif i == 5 or i == 6 or i == 7:
        laba = modal * 0.5   # 50% dari modal
    elif i == 8:
        laba = modal * 0.2   # 20% dari modal
    total += laba
    print(f"laba bulan ke-{i} sebesar: {laba}")

print(f"Total laba adalah: {total}")

Alur Algoritma
1. Tentukan modal awal = 100 juta.
2. Gunakan perulangan for dari bulan 1 sampai 8.
3. Gunakan logika percabangan untuk menentukan laba tiap bulan:
Bulan 1–2 → 0%
Bulan 3–4 → 10%
Bulan 5–7 → 50%
Bulan 8 → 20%
4. Setiap laba bulanan ditambahkan ke total.
5. Tampilkan laba tiap bulan dan total akhir.

Hasil Screenshot
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/d8b56fee-6e9d-4b34-b6c1-a99ecbbd349a" />


