# Belajar Git

## Menginisialisasi folder dengan git

tujuan inisisalisasi git supaya git mengetahui folder mana yang akan dipantau oleh git

```
git init
```

dengan ini maka folder yang kamu init sudah dipantau perubahannya oleh git

## Stage

```
git add .
```

maka semua file akan di stage

## Commit

```
git commit -m "pesan commit"
```

jika ingin stage dan juga commit maka menggunakkan perintah

```
git commit -am "pesan commit"
```

## Membuat branch/cabang

```
git branch nama_branch
```

## Pindah branch

```
git checkout nama_branch
```

## Push

```
git push
```

untuk push ke github bisa menggunakkan perintah dibawah

```
git push -u nama_remote nama_branch
contoh: git push -u origin master
```

## Push semua file dan branch

```
git push --all nama_remote
contoh: push --all origin
```

## Menambahkan remote

```
git remote add nama_remote url_repository
contoh: git remote add origin https://github.com/userexample/example.git
```

## Menghapus remote

```
git remote remove nama_remote
contoh: git remote remove origin
```

## Mengubah remote

```
git remote set-url nama_remote url_baru
git remote set-url origin git://new.url.here
```
