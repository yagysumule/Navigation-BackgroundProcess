# Tujuan
Pada latihan kali ini kita akan mencoba menerapkan skenario yang mirip dengan kejadian pada gambar berikut:

![MyDeepNavigation](https://user-images.githubusercontent.com/68750843/116654269-00a53800-a9b3-11eb-8e58-c6bde254211f.png)

Pada skenario di atas ketika pengguna menakan tombol membuat email baru, maka pengguna akan diarahkan ke activity yang bernama __ComposeActivity__. Di Activity ini, ketika pengguna menekan tombol _up button_, maka pada halaman utama aplikasi akan tampil __InboxActivity__. Hal yang sama akan terjadi bila pada __ComposeActivity__, pengguna menekan system back button. __InboxActivity__ akan ditampilkan pula.

Perbedaan baru muncul ketika pengguna berada di halaman utama, __InboxActivity__. Hanya _system back button_ saja yang dapat digunakan untuk menutup aplikasi. Ketika tombol ini ditekan, maka activity utama akan dihancurkan. Semua _task_ yang dimiliki aplikasi akan dihapus dari memori. Di tahap akhir, pengguna akan dikembalikan ke halaman _home screen_ dari perangkat Androidnya.

Alur di atas tidak hanya berlaku pada widget saja. Ia juga dapat terjadi pada notifikasi. Ketika terjadi pada notifikasi, mekanisme tersebut bernama _deeplink_.

Pada codelab kali ini, Anda akan membuat aplikasi seperti berikut:

![MyDeepNavigation](https://user-images.githubusercontent.com/68750843/116654521-80cb9d80-a9b3-11eb-9bd7-57fe7f4eb97b.gif)

# Logika Dasar
Muncul notifikasi → klik notifikasi → masuk ke dalam detail aplikasi → kembali ke halaman utama.