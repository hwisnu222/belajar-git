# Belajar Git

### Menginisialisasi folder dengan git

tujuan inisisalisasi git supaya git mengetahui folder mana yang akan dipantau oleh git

```
git init
```

dengan ini maka folder yang kamu init sudah dipantau perubahannya oleh git

### Stage

```
git add .
```

maka semua file akan di stage

### Commit

```
git commit -m "pesan commit"
```

jika ingin stage dan juga commit maka menggunakkan perintah

```
git commit -am "pesan commit"
```

### Membuat branch/cabang

```
git branch nama_branch
```

### Pindah branch

```
git checkout nama_branch
```

### Push

```
git push
```

untuk push ke github bisa menggunakkan perintah dibawah

```
git push -u nama_remote nama_branch
contoh: git push -u origin master
```

### Push semua file dan branch

```
git push --all nama_remote
contoh: push --all origin
```

### Menambahkan remote

```
git remote add nama_remote url_repository
contoh: git remote add origin https://github.com/userexample/example.git
```

### Menghapus remote

```
git remote remove nama_remote
contoh: git remote remove origin
```

### Mengubah remote

```
git remote set-url nama_remote url_baru
git remote set-url origin git://new.url.here
```

## Membatalkan revisi

Terkadang saat melakukan perubahan terhadap suatu file muncul keinginan untuk membatalkan revisi pada file tersebut . dibawah ini adalah cara untuk membatalkan file yang sudah di stage dan commit ataupun sebelumnya

### Membatalkan perubahan sebelum melakukan stage dan commit

```
git checkout nama_file

contoh: git checkout index.html
```

### Membatalkan perubahan file yang sudah dalam kondisi Stage, tapi belum dilakukan commit

```
git reset

atau

git reset nama_file

contoh: git reset index.html
```

### Mengembalikan perubahan file dalam keadaan sudah dicommit

yang perlu diperhatikan disini adalah harus mengetahui nomor commit yang ingin kita batalkan. setelah mengetahui nomor commitnya gunakkan perintah dibawah

```
git checkout nomor_commit

contoh: git checkout 344543253425rdt14s3trs431rs
```

setelah melakukan perintah diatas, maka file masih dalam keadaan stage, yang perlu dilakukan lagi adalah mengembalikan dalam keadaan modified. gunakkan perintah dibawah

```
git reset
```

### mengembalikan ke 3 commit sebelumnya

```
git checkout HEAD~3
```

### Membatalkan semua perubahan

```
git revert -n nomor_commit

contoh: git revert -n 4214g14hg15cgc152jh523gh5
```
