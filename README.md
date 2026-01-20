# 📚 Latihan Interview JavaScript - SOAL

---

## 🧮 Challenge 1: Array Methods (Variasi)

### Soal 1A: Hitung Rata-Rata dari Bilangan Genap Saja

Diberikan sebuah array angka, hitung rata-rata hanya dari bilangan **genap** saja.

**Contoh Input:**
```javascript
const arr = [10, 15, 20, 25, 30, 35, 40];
```

**Expected Output:**
```
25 // (10 + 20 + 30 + 40) / 4 = 100 / 4 = 25
```

---

### Soal 1B: Cari Nilai Minimum dan Maksimum Sekaligus

Diberikan sebuah array angka, kembalikan objek yang berisi nilai minimum dan maksimum **tanpa menggunakan Math.min() atau Math.max()**.

**Contoh Input:**
```javascript
const arr = [45, 12, 78, 3, 56, 99, 23];
```

**Expected Output:**
```javascript
{ min: 3, max: 99 }
```

---

### Soal 1C: Hitung Median dari Array

Diberikan sebuah array angka yang tidak terurut, hitung nilai **median** (nilai tengah).

**Aturan:**
- Jika jumlah elemen ganjil, median adalah nilai tengah
- Jika jumlah elemen genap, median adalah rata-rata dari 2 nilai tengah

**Contoh Input:**
```javascript
const arr1 = [3, 1, 4, 1, 5];  // setelah sort: [1, 1, 3, 4, 5]
const arr2 = [3, 1, 4, 1, 5, 9]; // setelah sort: [1, 1, 3, 4, 5, 9]
```

**Expected Output:**
```
arr1 → 3 (nilai tengah)
arr2 → 3.5 (rata-rata dari 3 dan 4)
```

---

### Soal 1D: Cari Nilai yang Muncul Paling Sering (Mode)

Diberikan sebuah array angka, kembalikan nilai yang paling sering muncul (mode).

**Contoh Input:**
```javascript
const arr = [1, 2, 2, 3, 3, 3, 4, 4];
```

**Expected Output:**
```
3 // muncul 3 kali
```

---

### Soal 1E: Hitung Jumlah Elemen Unik

Diberikan sebuah array, hitung berapa banyak elemen **unik** (tidak duplikat).

**Contoh Input:**
```javascript
const arr = [1, 2, 2, 3, 4, 4, 4, 5];
```

**Expected Output:**
```
5 // elemen unik: 1, 2, 3, 4, 5
```

---

## 🔤 Challenge 2: String Compression (Variasi)

### Soal 2A: String Compression dengan Lowercase

Sama seperti challenge asli, tapi hasil kompresi harus dalam **lowercase**.

**Contoh Input:**
```javascript
const str1 = 'AAAABBBCCCAA';
const str2 = 'AAAaaBBBbb';
```

**Expected Output:**
```
str1 → 'a4b3c3a2'
str2 → 'a3a2b3b2'
```

---

### Soal 2B: String Decompression (Kebalikan dari Compression)

Diberikan string yang sudah terkompresi, kembalikan ke bentuk aslinya.

**Contoh Input:**
```javascript
const compressed = 'A4B3C3A2';
```

**Expected Output:**
```
'AAAABBBCCCAA'
```

---

### Soal 2C: Run-Length Encoding dengan Karakter Tunggal Tanpa Angka

Modifikasi kompresi string: jika karakter hanya muncul **1 kali**, jangan tambahkan angka.

**Contoh Input:**
```javascript
const str1 = 'AAABBCDDD';
const str2 = 'ABCDEF';
```

**Expected Output:**
```
str1 → 'A3B2CD3'
str2 → 'ABCDEF' (original, karena tidak ada pengulangan)
```

---

### Soal 2D: Validasi String Terkompresi

Buat fungsi untuk memvalidasi apakah string kompresi valid (format: huruf diikuti angka positif).

**Aturan:**
- Hanya boleh huruf (A-Z, a-z) diikuti angka positif
- Tidak boleh ada karakter spesial
- Angka tidak boleh 0 atau negatif

**Contoh:**
```javascript
'A4B3C2'  → true
'A0B3'    → false (angka 0)
'4AB3'    → false (dimulai dengan angka)
'A-2B3'   → false (angka negatif)
'A4B'     → false (tidak ada angka setelah B)
```

---

### Soal 2E: Kompresi dengan Separator

Buat kompresi string dengan format berbeda: setiap grup dipisahkan dengan koma.

**Contoh Input:**
```javascript
const str = 'AAABBBCCAA';
```

**Expected Output:**
```
'A:3,B:3,C:2,A:2'
```

---

## 🎯 Bonus Challenge: Kombinasi Array & String

### Soal Bonus: Analisis Array of Strings

Diberikan array of strings, kembalikan statistik berikut:
- Total karakter di semua string
- String terpanjang
- String terpendek
- Rata-rata panjang string

**Contoh Input:**
```javascript
const arr = ['hello', 'world', 'javascript', 'code'];
```

**Expected Output:**
```javascript
{
  totalChars: 24,
  longest: 'javascript',
  shortest: 'code',
  averageLength: 6
}
```

---

## 📋 Tips untuk Interview

1. **Selalu tanyakan edge cases** - Array kosong? String kosong? Angka negatif?
2. **Jelaskan pendekatan sebelum coding** - Interviewer ingin tahu proses berpikir Anda
3. **Tulis test cases** - Tunjukkan bahwa Anda memikirkan berbagai skenario
4. **Mulai dengan solusi sederhana** - Optimize kemudian jika diperlukan
5. **Gunakan nama variabel yang jelas** - `count` lebih baik dari `c`

---

