# **Tugas Praktikum 4 – labpy03**

# *Latihan 1 - Bilangan Acak Kurang dari 0.5 *

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
