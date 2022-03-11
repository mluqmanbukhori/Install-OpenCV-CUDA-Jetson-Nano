# Install OpenCV versi 4.5.0 CUDA di Jetson Nano
Repositori ini digunakan untuk melakukan install OpenCV versi 4.5.0 dengan mengaktifkan CUDA Compiled di Jetson Nano. Lihat Gambar berikut ini.<br><br>
![OpenCV](https://github.com/mluqmanbukhori/Install-OpenCV-CUDA-Jetson-Nano/blob/main/OpenCV-CUDA.jpg)

# Persiapan sebelum Install
Sebelum melakukan installasi Opencv with CUDA di Jetson Nano Anda, pastikan sudah menginstall `Qt5` menggunakan script berikut.
> **Catatan:** Jika sudah menginstall bisa melewati langkah ini
<div><pre>
  $ sudo apt-get install -y qt5-default
</pre></div>

# Mulai Install OpenCV
* Download script `OpenCV_4-5-0_CUDA.sh` yang telah disiapkan dengan cara berikut
<div><pre>
  $ wget https://github.com/mluqmanbukhori/Install-OpenCV-CUDA-Jetson-Nano/raw/main/OpenCV_4-5-0_CUDA.sh
</pre></div>

* Atur otoritas file dengan `chmod`
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
