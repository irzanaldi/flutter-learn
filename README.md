# Flutter

> Kumpulan project pembelajaran (learning) Flutter. Folder ini menampung beberapa sub-project Flutter yang berdiri sendiri.

## Sub-project

| Folder | Keterangan | Status git |
|--------|-----------|------------|
| `app_user_clone/` | Latihan clone aplikasi user | repo git tersendiri (embedded) |
| `prototype-bidan-mobile-main/` | Prototype app bidan (Flutter + GetX) | repo git tersendiri (embedded) |
| `test_project/flutter_application_1/` | Project starter Flutter | bagian dari repo ini |

> Catatan: `app_user_clone/` dan `prototype-bidan-mobile-main/` punya folder `.git` sendiri, sehingga di repo ini tercatat sebagai *embedded repository* (penunjuk submodule), bukan sebagai isi filenya.

## Cara Setup

Prasyarat:
- Flutter SDK terpasang (`flutter --version`)
- Emulator/device Android atau iOS, atau Chrome untuk target web

Langkah (jalankan di dalam folder sub-project, contoh `test_project/flutter_application_1`):

1. Masuk ke folder sub-project:
   ```bash
   cd "Flutter/test_project/flutter_application_1"
   ```

2. Ambil dependency:
   ```bash
   flutter pub get
   ```

3. Cek device yang tersedia:
   ```bash
   flutter devices
   ```

4. Jalankan aplikasi:
   ```bash
   flutter run
   ```

5. Jalankan test:
   ```bash
   flutter test
   ```

> Untuk sub-project lain (`app_user_clone`, `prototype-bidan-mobile-main`) langkahnya sama: masuk ke foldernya lalu `flutter pub get` dan `flutter run`.
> `prototype-bidan-mobile-main` memakai Firebase; file `android/app/google-services.json` sengaja di-*ignore* demi keamanan — siapkan file Firebase Anda sendiri bila ingin menjalankannya.
