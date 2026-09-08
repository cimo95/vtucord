---
description: '@everyone dan @here, (termasuk kata terlarang lainnya)'
---

# Mencegah mass-mention dan kata terlarang

### Deskripsi

Apa itu mass-mention? Mass-mention adalah penyebutan (mention) yang akan memanggil seluruh anggota server (@everyone), atau setidaknya anggota yang sedang online/aktif saat itu (@here).

Hal ini sering terjadi dan dilakukan mulai dari member server yang iseng, hingga spammer/scammer. Sebenarnya, tidak ada alasan untuk member non-staff melakukan mass-mention selain hanya akan mengganggu member lain. Oleh karena itu, akan kita bahas cara mencegah penggunaan mass-mention ini oleh non-staff, dan memberikan peringatan serta timeout pada mereka.

Di sini kita akan memanfaatkan fitur AutoMod "Block Custom Words" di mana kita bisa mengatur kata-kata apa saja yang tidak boleh dikirimkan ke chat di server.

{% hint style="warning" %}
Jika kamu bukan pemilik server, tanyakan pada pemilik server untuk memastikan role kamu setidaknya memiliki permission "Manage Server".

![](../../.gitbook/assets/{A6EFA105-498A-4D53-9F56-F8C2A15F72A1}.png)
{% endhint %}

### Versi Desktop / Browser

{% stepper %}
{% step %}
### Buka "Server Settings"

Buka menu server dengan mengklik judul server, lalu pilih "Server Settings"

<figure><img src="../../.gitbook/assets/{F55D2A85-8B9E-4448-93B8-3E3843F7D544}.png" alt="" width="185"><figcaption><p>Letak "Server Settings"</p></figcaption></figure>
{% endstep %}

{% step %}
### Buka "Safety Setup"

Setelah tampilan "Server Settings" muncul, di baris menu kiri, pilih "Safety Setup"
{% endstep %}

{% step %}
### Edit "AutoMod"

Setelah tampilan "Safety Setup" muncul, klik "Edit" pada blok "AutoMod"

<figure><img src="../../.gitbook/assets/image.png" alt="" width="537"><figcaption><p>Letak "AutoMod" di "Safety Setup"</p></figcaption></figure>
{% endstep %}

{% step %}
### Buat aturan baru

Pada tampilan "AutoMod", di bagian "Content" klik "Create" pada blok aturan "Block Custom Words"

<figure><img src="../../.gitbook/assets/image (1).png" alt="" width="536"><figcaption><p>Letak "Block Custom Words" di "AutoMod"</p></figcaption></figure>
{% endstep %}

{% step %}
### Isikan `*@everyone*` dan `*@here*`

* Kamu bisa mengubah nama rule ini di "Rule Name"
* Ketik `*@everyone*` dan `*@here*` di bagian "Choose your words" dipisah dengan koma.

<figure><img src="../../.gitbook/assets/image (2).png" alt="" width="507"><figcaption><p>Mengisi kata yang diblokir di bagian "Choose your words"</p></figcaption></figure>

{% hint style="success" %}
**Kenapa harus diapit dengan bintang?**

Dengan mengapit kata dengan tanda bintang, kita menjelaskan pada AutoMod bahwa tidak hanya kata yang berdiri sendiri yang akan dikenai aturan, tapi juga bagian dari kata-katanya.

Ini berarti, berlaku juga untuk kata apa pun.

Misal, dengan mengisikan `*babi*` kita tidak hanya memblokir kalimat :\
`babi itu jorok` tapi juga `hewan itu membabi buta` .

Perhatikan, kalimat pertama `babi` berdiri sendiri (dipisah spasi), dan kalimat kedua `babi` memiliki awalan `mem` .
{% endhint %}
{% endstep %}

{% step %}
### Atur tindakan AutoMod

Di bagian "Choose a response" pilih apa saja yang akan dilakukan AutoMod, jika terdapat member yang mengirimkan mass-mention

<figure><img src="../../.gitbook/assets/{8717688B-B11A-4CE0-A5CA-A46408D77750}.png" alt="" width="514"><figcaption><p>Tampilan tindakan AutoMod jika terpicu</p></figcaption></figure>

* **Block message**\
  Chat member yang mengandung mass-mention akan dibatalkan, dan AutoMod menampilkan pesan khusus. Pesan ini bisa kamu ubah di "Edit Custom Message".

<figure><img src="../../.gitbook/assets/{5A47E434-3899-44DE-9DD7-68E1DCB82FCE}.png" alt=""><figcaption><p>Contoh pesan khusus yang muncul ke member.</p></figcaption></figure>

* **Send Alert**\
  AutoMod akan mencatat pelanggaran ini ke suatu channel sebagai riwayat tindakan.

<figure><img src="../../.gitbook/assets/{E18F1189-4269-4B66-B06E-02D62E2D0209}.png" alt="" width="451"><figcaption><p>Tampilan riwayat tindakan AutoMod</p></figcaption></figure>

* **Time out member**\
  AutoMod akan men-TO (timeout) member yang melakukan pelanggaran sesuai durasi yang ditentukan. Durasi ini bisa kamu ubah di "Edit Duration".

<figure><img src="../../.gitbook/assets/{7E498BF9-EB2E-4EBB-9638-3CBD3A4212BC}.png" alt=""><figcaption><p>Tampilan member yang di-TO</p></figcaption></figure>

{% hint style="danger" %}
Jika "Block message" tidak diaktifkan, meski "Send alert" atau "Time out member" diaktifkan, pesan tidak akan ditahan, dan tetap muncul di riwayat chat.
{% endhint %}
{% endstep %}

{% step %}
### Atur pengecualian

Pilih role dan/atau channel mana saja yang tidak akan dikenai aturan ini.

Jadi, jika mention dilakukan di channel ini, atau oleh member dengan role yang ada pada daftar ini, AutoMod tidak akan terpicu.

<figure><img src="../../.gitbook/assets/{F5E794D1-EDF0-4505-8889-3B25F947ADAE}.png" alt="" width="515"><figcaption><p>Tampilan channel dan role yang dikecualikan</p></figcaption></figure>
{% endstep %}

{% step %}
### Simpan

Jangan lupa untuk selalu menyimpan perubahan yang sudah dibuat dengan mengklik "Save Changes".

<figure><img src="../../.gitbook/assets/{FEF28B2B-6AC7-45EC-A458-747D60142B97}.png" alt="" width="518"><figcaption><p>Tampilan bilah "Save Changes"</p></figcaption></figure>
{% endstep %}
{% endstepper %}

{% hint style="warning" %}
Hati-hati, agar tidak menutup blok rule yang sedang kamu kerjakan.\
Menutup blok ini sama saja dengan membatalkan perubahan yang ada.
{% endhint %}

{% hint style="success" %}
Kamu juga bisa menambahkan role dan member server untuk dicegah penyebutannya dengan cara menambahkan `*<@&Role ID>*` dan `*<@User ID>*` di bagian "Choose your words".

<img src="../../.gitbook/assets/{B1115DDE-ECC6-4056-9C17-00F196DA5AAC}.png" alt="" data-size="original">

Role ID bisa didapatkan dengan [mengaktifkan Developer Mode](mengaktifkan-developer-mode.md) terlebih dahulu, lalu buka "Roles" di "Server Settings", klik elipsis (titik tiga) di baris role yang akan diambil IDnya, lalu klik "Copy Role ID"

![](<../../.gitbook/assets/{4B1FA9F0-0899-4446-BD18-D76F2C85C740} (1).png>)

User ID bisa didapatkan dengan [mengaktifkan Developer Mode](mengaktifkan-developer-mode.md) terlebih dahulu, lalu klik kanan pada member yang ingin disalin User IDnya, lalu klik "Copy User ID"
{% endhint %}

### Versi Mobile

Untuk saat ini, agar mendapatkan hasil yang sama, gunakan Discord melalui browser perangkat mobile.
