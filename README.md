# SIC6_UNI227
Assignment Stage 3

---

# 🗑️ Smart Dustbin with Arduino Uno & ESP32-CAM
# 📌 Description
      Smart Dustbin adalah sistem tempat sampah pintar yang dapat membuka tutup otomatis berdasarkan jenis sampah yang dikenali melalui kamera (ESP32-CAM) dan menggerakkan servo menggunakan Arduino Uno. Proyek ini bertujuan untuk meningkatkan efisiensi dalam pemilahan sampah serta mengurangi kontak langsung dengan tempat sampah.

# 🛠️ Hardware Components
  - ESP32-CAM
  - Arduino Uno
  - Servo motor
  - Kabel jumper
  - Kabel USB
  - OLED Display
  - Breadboard
  - Power supply (opsional)

# ⚙️ System Workflow
  1. ESP32-CAM mengambil gambar sampah yang dimasukkan ke dalam tempat sampah.
  2. Gambar dikirim ke model klasifikasi (*pre-trained model* dari Edge Impulse) untuk mengenali jenis sampah: organik, anorganik, atau B3.
  3. Hasil klasifikasi dikirim ke Arduino Uno.
  4. Arduino Uno mengontrol servo motor untuk membuka tutup tempat sampah sesuai jenis sampah yang terdeteksi.
  5. Informasi ditampilkan di OLED display atau dikirim ke platform monitoring.

# 🧠 ML Inference
  Model klasifikasi sampah dilatih menggunakan Edge Impulse dan di-deploy ke ESP32-CAM untuk inferensi gambar secara real-time.

# 💡 Features
  - Deteksi otomatis jenis sampah (organik, anorganik, B3)
  - Buka tutup otomatis via servo
  - Minim kontak fisik
  - Potensial untuk integrasi IoT (monitoring data, notifikasi, dsb.)

# 👨‍💻 How to Use
  1. Upload firmware klasifikasi gambar ke ESP32-CAM.
  2. Upload kode Arduino ke Arduino Uno untuk kontrol servo.
  3. Sambungkan semua komponen sesuai skema rangkaian.
  4. Nyalakan sistem, arahkan sampah ke depan kamera, dan lihat respon tempat sampah.

# NB:
  - Karena ini masih berupa prototype --terkendala waktu, biaya, dan juga banyaknya bug, kami hanya mampu membuat program sederhana dari pengimplementasian smart-dustbin berintegrasikan sensor dan servo. harapannya, ini bisa menjadi pembelajaran kami kedepannya untuk lebih berinovasi dengan program yang ingin kami buat.
---
