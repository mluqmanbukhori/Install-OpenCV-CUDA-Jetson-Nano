# Install OpenCV versi 4.5 CUDA di Jetson Nano
Repositori ini digunakan untuk melakukan install OpenCV versi 4.5.X dengan mengaktifkan CUDA Compiled di Jetson Nano. Lihat Gambar berikut ini.<br><br>
![OpenCV](https://github.com/mluqmanbukhori/Install-OpenCV-CUDA-Jetson-Nano/blob/main/OpenCV-CUDA.jpg)

# Persiapan sebelum Install
Sebelum melakukan installasi Opencv with CUDA di Jetson Nano Anda, pastikan sudah menginstall `Qt5` menggunakan script berikut.
> **Catatan:** Jika sudah menginstall bisa melewati langkah ini
<div><pre>
  $ sudo apt-get install -y qt5-default
</pre></div>

# Mulai Install OpenCV
Terdapat beberapa versi OpenCV yang bisa Anda download
  1. OpenCV_4-5-0_CUDA.sh
  2. OpenCV_4-5-1_CUDA.sh
  3. OpenCV_4-5-2_CUDA.sh
  4. OpenCV_4-5-3_CUDA.sh
  5. OpenCV_4-5-4_CUDA.sh
  6. OpenCV_4-5-5_CUDA.sh
* Download script `OpenCV_4-5-x_CUDA.sh` yang telah disiapkan `ganti x dengan versi yang diinginkan` dengan cara berikut
<div><pre>
  $ wget https://github.com/mluqmanbukhori/Install-OpenCV-CUDA-Jetson-Nano/raw/main/OpenCV_4-5-x_CUDA.sh
</pre></div>

* Atur otoritas file dengan `sudo chmod`
<div><pre>
  $ sudo chmod 755 ./OpenCV_4-5-0_CUDA.sh
</pre></div>

* Install OpenCV dengan menuliskan script berikut
> **Catatan:** Ketika install membutuhkan Koneksi yang Stabil dan Waktu yang ekstra +/- 3 Jam lamanya, mohon bersabar menunggu
<div><pre>
  $ ./OpenCV_4-5-0_CUDA.sh
</pre></div>

# Cek OpenCV CUDA dengan Jetson Stats 
Ketik di terminal `$ jtop`

# Kontribusi
Jangan lupa follow media Sosial kami <br>
YouTube : [Elektro Project](https://www.youtube.com/elektroproject) <br>
Twitter : [@mluqmanbukhori](https://twitter.com/mluqmanbukhori)
