# Ban user yang bukan member server

### Deskripsi

Tips ini berguna jika kamu ingin mencegah seseorang/user yang sudah kamu ketahui akun Discordnya, agar tidak bergabung ke server kamu/server yang kamu urus.

Tips ini membutuhkan User ID akun yang ingin kamu cegah. Discord secara default tidak menampilkan User ID di pop-up menu mereka. Maka dari itu, kita perlu mengaktifkannya terlebih dahulu, sebelum dapat mengambil User ID.

{% hint style="warning" %}
Jika kamu bukan pemilik server, tanyakan pada pemilik server untuk memastikan role kamu setidaknya memiliki permission "Ban Members".

![](../../.gitbook/assets/{F4A2EF8E-0D70-4057-8705-478CC73D7513}.png)
{% endhint %}

### Versi Desktop / Browser

{% stepper %}
{% step %}
### Aktifkan "Developer Mode"

Untuk dapat melakukan tindakan ini, kamu harus mengaktifkan "Developer Mode" terlebih dahulu.&#x20;

Petunjuk prosedur ini, tersedia di halaman "[Mengaktifkan Developer Mode](mengaktifkan-developer-mode.md)".
{% endstep %}

{% step %}
### Salin "User ID" akunnya

Klik kanan di profil akun target, lalu pilih "Copy User ID".

Kamu juga bisa menampilkan profil target terlebih dulu untuk memastikan, lalu klik titik tiga di pojok kanan atas tampilan profil target, dan klik "Copy User ID"

<figure><img src="../../.gitbook/assets/{3F83435B-08D9-4D28-BA66-822226430126}.png" alt=""><figcaption><p>Menyalin "User ID" dari akun Discord target</p></figcaption></figure>
{% endstep %}

{% step %}
### Jalankan perintah `/ban`&#x20;

Pergi ke sembarang Channel Text yang kotak chatnya mengizinkan pengiriman slash command (tekan tanda slash/garis miring `/` . Jika muncul daftar perintah bot/app, berarti slash command diizinkan.)

Ketik `/ban`, dari daftar perintah yang muncul, pilih yang built-in Discord (dengan ikon garis miring abu-abu).

<figure><img src="../../.gitbook/assets/tips-0000-0004.jpg" alt=""><figcaption><p>Letak perintah "/ban" built-in Discord</p></figcaption></figure>
{% endstep %}

{% step %}
### Masukkan User IDnya

Setelah dipilih, isi kotak "user" dengan "`<@>`".

<figure><img src="../../.gitbook/assets/{48A59731-992C-431B-8D6F-9DBFF7BC08BD}.png" alt=""><figcaption><p>Pengisian "&#x3C;@>" di kotak "user"</p></figcaption></figure>

Selanjutnya, tempel User ID yang sudah disalin tadi di antara tanda `@` dan `>` .\
Setelah itu, kotak "user" akan otomatis berubah ke username akun tersebut, atau muncul sebagai `unknown-user`, abaikan. Jika muncul `unknown-user` ini normal, karena user tersebut tidak berteman denganmu, atau tidak berada di server tersebut.

<figure><img src="../../.gitbook/assets/{6A470AB7-7DAF-4A12-ACBC-50717856C06E}.png" alt=""><figcaption><p>Kotak "user" setelah ditambahkan User ID di "&#x3C;@>"</p></figcaption></figure>

{% hint style="danger" %}
JANGAN menekan **Enter** saat berada di kotak "user" untuk menghindari secara tidak sengaja memilih butir user yang muncul di daftar.
{% endhint %}
{% endstep %}

{% step %}
### Lengkapi isian lainnya, dan selesaikan

Pilih "delete\_messages" dan sesuaikan pilihannya.

Pilih "+1 more" lalu pilih "reason" untuk mengisi alasan ban ini.

Setelah semua opsi terisi, tekan Enter untuk memproses ban.

<figure><img src="../../.gitbook/assets/{28ECB105-C1C1-411D-A4C7-8BB547ECCE73}.png" alt=""><figcaption><p>Perintah "/ban" dengan semua kotak sudah diisi</p></figcaption></figure>
{% endstep %}

{% step %}
### Selesai

Tunggu beberapa saat hingga pesan dari Clyde muncul.

<figure><img src="../../.gitbook/assets/{5A388783-2C49-45C1-A100-F3724C1B4FBB}.png" alt=""><figcaption><p>Pesan user berhasil diban</p></figcaption></figure>
{% endstep %}
{% endstepper %}

### Versi Mobile

Untuk saat ini, agar mendapatkan hasil yang sama, gunakan Discord melalui browser perangkat mobile.
