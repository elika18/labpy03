# **Tugas Praktikum 4**

# *Latihan 1 - Bilangan Acak Kurang dari 0.5*

```python
# Meminta input nilai N saat runtime
n = int(input("Masukkan nilai N: "))

i = 0
while i < n:
    a = random()  # menghasilkan angka acak antara 0 dan 1
    if a < 0.5:   # hanya tampilkan jika < 0.5
        print(f"data ke: {i+1} => {a}")
        i += 1

print("Selesai")
```
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
```python
# Modal awal
modal = 100000000

# Inisialisasi total laba
total = 0

#Perulangan selama 8 bulan
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
```
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

# *Latihan 3 – Simulasi Mesin ATM Sederhana*

Kode Program (latihan3.py)

saldo = 1000000  # saldo awal

while True:
    print(f"\nSaldo saat ini: Rp {saldo}")
    print("1. Tarik Uang")
    print("2. Keluar")
    pilihan = input("Pilih menu (1/2): ")

    if pilihan == "1":
        tarik = int(input("Masukkan jumlah penarikan: "))
        if tarik > saldo:
            print("Saldo tidak cukup!")
        elif tarik <= 0:
            print("Jumlah penarikan tidak valid!")
        else:
            saldo -= tarik
            print("Penarikan berhasil!")
    elif pilihan == "2":
        print("Terima kasih telah menggunakan ATM!")
        break
    else:
        print("Pilihan tidak valid, silakan coba lagi.")

Alur Algoritma
1. Inisialisasi saldo awal sebesar Rp1.000.000.
2. Program menampilkan dua menu:
(1) Tarik uang
(2) Keluar
3. Jika pengguna memilih 1, masukkan jumlah uang yang akan ditarik:
Jika jumlah lebih besar dari saldo → tampilkan pesan "Saldo tidak cukup".
Jika jumlah ≤ 0 → tampilkan pesan "Jumlah tidak valid".
Jika valid → saldo dikurangi dan tampil pesan "Penarikan berhasil".
4. Jika pengguna memilih 2, program berhenti dengan pesan "Terima kasih".
5. Jika pilihan tidak valid → tampilkan pesan kesalahan.

📸 Hasil Screenshot
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/6083becb-65e2-425d-b960-ca2d318d7cb9" />

# Kesimpulan

Latihan 1: Belajar penggunaan random() dan kontrol perulangan while.

Latihan 2: Memahami perulangan for dan logika percabangan untuk menghitung laba.

Latihan 3: Menerapkan konsep input, output, perulangan, dan kondisi pada simulasi ATM.
