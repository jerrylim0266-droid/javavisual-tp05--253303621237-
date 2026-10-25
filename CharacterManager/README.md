# Character Manager — TP3 (Java Visual SIH-6406)

Character Manager adalah aplikasi Java sederhana untuk membuat dan mengelola karakter game menggunakan konsep pemrograman berorientasi objek. Aplikasi ini memodelkan nama, jenis, level, HP, attack, dan mana karakter, serta menyediakan pemeriksaan status hidup melalui method `isAlive()`.

# Hasil Program terminal

Berikut screenshot hasil eksekusi aplikasi:

![Hasil eksekusi Character Manager](Screenshot.png)

# Fitur Analitik Rancangan Sendiri

Fitur tambahan yang dibuat adalah `renameCharacter(oldName, newName)` pada
`CharacterManager`. Method ini mengganti nama karakter yang sudah terdaftar,
tetapi hanya jika karakter dengan nama lama ditemukan dan nama baru tidak
kosong serta belum digunakan oleh karakter lain. Jika validasi gagal, method
mengembalikan `false` dan data karakter tidak diubah; jika berhasil,
mengembalikan `true`.

Fitur ini berguna untuk memperbarui nama karakter tanpa menghapus lalu membuat
karakter baru, sehingga tipe, level, dan atribut lainnya tetap dipertahankan.
Encapsulation tetap terjaga karena method bekerja langsung pada koleksi internal
`CharacterManager` tanpa mengembalikan atau mengekspos `ArrayList` tersebut.
Pengujiannya di `Main.java` menunjukkan bahwa penggantian nama Merlin menjadi
Arjuna ditolak karena nama Arjuna sudah dipakai, sedangkan penggantian Merlin
menjadi Gandalf berhasil.



# Struktur Folder Project

```text
CharacterManager/
├── images/
│   ├── README.md
│   └── Screenshot.png
└── src/
    ├── Main.java
    └── com/
        └── unpri/
            └── charactermanager/
                └── model/
                    ├── Character.java
                    ├── CharacterManager.java
                    └── CharacterType.java
```
# Identitas Mahasiswa

- Nama Lengkap:JERRY LIM
- NIM:253303621237
- Google Docs — TP3 Bagian D:[Buka dokumen Google Docs](https://docs.google.com/document/d/1QCCENsT26y548l06515b_NNMhOVXbDBsuPcFhBB3kfo/edit?usp=sharing)
              — TP5 Bagian D:[Buka dokumen Google Docs](https://docs.google.com/document/d/1U4AAVVxghHRqwvg9p-WrIZhaKMxz98BZm47wv41bs3c/edit?usp=sharing)