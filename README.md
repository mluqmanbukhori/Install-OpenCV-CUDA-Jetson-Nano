# Install OpenCV versi 4.5.X CUDA di Jetson Nano
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
  $ sudo chmod 755 ./OpenCV_4-5-x_CUDA.sh
</pre></div>

* Install OpenCV dengan menuliskan script berikut
> **Catatan:** Ketika install membutuhkan Koneksi yang Stabil dan Waktu yang ekstra +/- 3 Jam lamanya, mohon bersabar menunggu
<div><pre>
  $ ./OpenCV_4-5-x_CUDA.sh
</pre></div>

# Cek CUDA Installation L4T
ketik di terminal `$ nvcc --version` <br>
Jika `nvcc: error` perlu melakukan instruksi berikut
<div><pre>
  masuk ke folder src
  $ cd /usr/local/src 
  <br>copy path CUDA dengan mengetik line berikut
  $ echo "export PATH=/usr/local/cuda/bin${PATH:+:${PATH}}" >> ~/.bashrc
  $ echo "export LD_LIBRARY_PATH=/usr/local/cuda/lib64${LD_LIBRARY_PATH:+:${LD_LIBRARY_PATH}}" >> ~/.bashrc
  <br>compile bashrc file
  $ source ~/.bashrc
  <br>cek PATH environment
  $ dpkg -l | grep cuda
  <br>cek NVCC
  $ nvcc --version
</pre></div>

Tampilan yang muncul ketika mengetikan `nvcc --version` kurang lebih seperti berikut
> **Catatan:** setiap model Jetson berbeda tergantung versi yang terinstall dari Jetpack 
<div><pre>
  nvcc: NVIDIA (R) Cuda compiler driver
  Copyright (c) 2005-2021 NVIDIA Corporation
  Built on Sun_Feb_28_22:34:44_PST_2021
  Cuda compilation tools, release 10.2, V10.2.300
  Build cuda_10.2_r440.TC440_70.29663091_0
</pre></div>

# Cek OpenCV CUDA dengan Jetson Stats 
Ketik di terminal `$ jtop` <br>
Jika `Error` berarti belum terinstall, ikuti langkah berikut
<div><pre>
  $ sudo -H pip install -U jetson-stats
  $ sudo reboot
</pre></div>

Ketikan kembali di terminal `$ jtop`

# Kontribusi | Mau bertanya?
Jangan lupa follow media Sosial kami <br>
YouTube : [Elektro Project](https://www.youtube.com/elektroproject) <br>
Twitter : [@mluqmanbukhori](https://twitter.com/mluqmanbukhori) <br>
Instagram : [@mluqmanbukhori](https://instagram.com/mluqmanbukhori) | [@elektro.project](https://instagram.com/elektro.project)
