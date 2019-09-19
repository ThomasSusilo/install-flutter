# Install Flutter di Windows Tanpa Android Studio

Untuk melakukan Instalasi <b>Flutter</b> pada Windows cukup mudah. Namun pastikan Windows Anda sudah memenuhi syarat. Berikut adalah beberapa rekomendasi yang dibutuhkan.

1. Microsoft Windows 7 SP1 atau diatasnya, direkomendasikan <b>Windows 10</b>.
2. Disk Spcae <b>400MB</b>.
3. <b>Windows PowerShell 5.0</b> atau diatasnya (Sudah include di Windows 10).
4. Jika Anda menggunakan Windows 7 atau Windows 8, Anda harus menginstall Windows PowerShell terlebih dahulu, silahkan mengikuti artikel di halaman <a href="https://docs.microsoft.com/en-us/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-windows-powershell-5-1"> Doc Microsoft </a>.
5. <b> Git </b> untuk Windows versi 2.0 atau diatasnya.

## Install JDK
Cek apakah ada JDK/JRE sudah terinstall sebelumnya (atau bawaan mesin). Uninstall agar bersih via: <b> Control Panel > Programs > Programs and Features </b>.

Download JDK 11.* terbaru ( saya lebih prefer versi stabil 8.* ) di <a href="https://www.oracle.com/technetwork/java/javase/downloads/index.html"> https://www.oracle.com/technetwork/java/javase/downloads/index.html </a>

<img src ="flutter1.png">

Klik file installer yang sudah di donwload. Di wizard instalasi jangan lupa sempatkan catat/copy instalasi kita, contoh <code>C:\Program Files\Java\jdk1.8.0_191\ </code>(yang nanti akan menjadi JAVA_HOME)

<img src="javaJDK.png">

Setelah terinstall, buka : <code>Control Panel > System and Security > System > Advanced System Setting</code> lalu pilih <b> Tab Advanced </b> dan klik tombol <b> Environtment Variables </b>.

<img src ="envi.png">

Cari bagian Path lalu edit atau tambahkan <code>C:\Program Files\Java\jdk.1.8.0_191\bin;</code> (dipaling depan saja), lalu klik OK.

<img src ="path.png">

Untuk memeriksa apakah path kita sudah siap dipalai, buka <b>Command Shell</b> dan cek versi Java menggunakan Command Line: <code>Java -version</code>

<img src = "javaVersion.png">

Kembali ke <b>Environment Variables</b>, gunakan tombol New dan buat variabel JAVA_HOME dengan isi Path JDK (tanpa bin).

<img src = "javaHome.png">

Buka Command Shell baru lagi dan periksa dengan Command : <code>SET JAVA_HOME</code>

<img src ="SetjavaHome.png">

## Install Gradle
Download Gradle (versi 3.5.x, pilih-pilih sehingga tidak perlu dokumentasi dan source) dari <a href="https://gradle.org/next-steps/?version=3.5&format=bin"> https://gradle.org/next-steps/?version=3.5&format=bin </a> lalu alamat Directory atau Path Gradle kita set menjadi <b>GRADLE_HOME</b>.

<img src ="gridle1.png">

Jangan lupa tambahkan juga (dengan /bin) ke Path Windows.

<img src ="gridle2.png">

Buka Command Shell baru dan Test Gradle sudah berjalan atau belum, dengan menuliskan Command : <code>gradle -v</code>

<img src ="gridle3.png">

## Install Android Command Line Tools
Download Android command line tools-nya saja dari, <a href="https://developer.android.com/studio/#downloads">https://developer.android.com/studio/#downloads</a>

<img src ="linetool1.png">

Ekstrak /tools ke direktori (kita ikuti path Android Studio saja) <code>C:\Users\nama_user\AppData\Local\Android\Sdk\tools</code>.

<img src ="linetool2.png">
<img src ="linetool3.png">
<img src ="linetool4.png">
<img src ="linetool5.png">

## Download Git For Windows

Download dan ekstrak Flutter SDK, tambahkan juga pathnya

<img src = "git1.png">

Install USB Driver untuk device Android kita di <a href="https://developer.android.com/studio/run/oem-usb">https://developer.android.com/studio/run/oem-usb</a>, aktifkan Developer & Debug Mode lalu sambungkan device ke laptop kita.

Jalankan Command Flutter Doctor

<img src ="git2.png">

Flutter telah siap digunakan.

# Info Lanjut
<a href="http://www.matanauniversity.ac.id/"> MATANA UNIVERSITY </a>
