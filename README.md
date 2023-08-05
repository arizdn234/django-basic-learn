# **Markdown Repeater for Django 4.2.2 project**

## Instalasi

1. Instal Python | (download lalu instal)
2. Instal Pip | (umumnya sudah terinstal jika sudah instal python)
3. Instal Django | gunakan terminal ->

```sh
    pip install Django
```

> [!NOTE]
> kemungkinan langkah instalasi Django bisa berubah, jadi lebih baik cek dulu di dokumentasinya -> [How to install Django?](https://docs.djangoproject.com/en/topics/install/)

## Setup awal

1. Inisiasi project dengan membuat folder dengan 'nama_project' ->

```sh
    mkdir nama_project
```

2. Ubah lokasi ke direktori project ->

```sh
    cd nama_project
```

3. Inisiasi Framework Django ke project ->

```'sh
    django-admin startproject project .
```

4. Inisiasi App ke project ->

```sh
    python manage.py startapp app
```

5. Test aplikasi dengan menjalankan server ->

```sh
    python manage.py runserver
```

> [!NOTE]
> kemungkinan perintah inisiasi project bisa berubah, jadi lebih baik cek dulu di dokumentasinya -> [Writing your first Django app](https://docs.djangoproject.com/en/4.2/intro/tutorial01/)

## Inisiasi App

1. Setup applikasi yang telah dibuat di `'project > settings.py > INSTALLED_APPS'`
2. Daftarkan url app ke project `'project > urls.py > urlpatterns'`

## Inisiasi model

1. Setup database yang digunakan di `'project > settings.py > DATABASES'`
2. Buatlah model dari database dengan inisiasi class dari tabel yang dibutuhkan pada file `'app > models.py'`
3. Inisiasi model yang telah dibuat ->

```sh
    python manage.py makemigrations
```

4. Checkout model yang telah diinisiasi ->

```sh
    python manage.py migrate
```

> [!NOTE]
> kemungkinan cara pembuatan model bisa berubah, jadi lebih baik cek dulu di [Database setup](https://docs.djangoproject.com/en/4.2/intro/tutorial02/)

## Inisiasi view dan form

1. Buat template view project di `'project > templates > site > index.html'`
2. Daftarkan template ke django `'project > settings.py > TEMPLATES'`
3. Buat template view app di `'app > templates > exampleApp > index.html'`
4. Buat form jika membutuhkan form di `'app > forms.py'`
5. Inisiasi template view dan form di `'app > views.py'`
6. Jangan lupa masukkan viewsnya ke `'app > urls.py > urlpatterns'`
   > [!NOTE]
   > kemungkinan cara pembuatan view bisa berubah, jadi lebih baik cek dulu di [Create view](https://docs.djangoproject.com/en/4.2/intro/tutorial03/)

## Inisiasi admin panel

1. Daftarkan model app ke admin site di `'app > admin.py'`
2. Buat kredensial login admin site ->

```sh
    python manage.py createsuperuser
```

> [!NOTE]
> kemungkinan cara pembuatan admin panel bisa berubah, jadi lebih baik cek dulu di [Admin setup](https://docs.djangoproject.com/en/4.2/intro/tutorial02/)

## Daftar list command

| Perintah                            | Fungsi                        |
| :---------------------------------- | :---------------------------- |
| `mkdir your-django-project`         | membuat direktori folder      |
| `cd your-django-project`            | masuk ke direktori            |
| `django-admin startproject project` | install django/create project |
| `python manage.py startapp app`     | membuat app                   |
| `python manage.py makemigrations`   | setup database                |
| `python manage.py migrate`          | checkout database             |
| `python manage.py createsuperuser`  | membuat superuser             |
| `python manage.py runserver`        | menjalankan server            |