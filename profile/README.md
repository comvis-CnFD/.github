# Crowd and Fatigue Detection System
## 📖 Overview

**Crowd and Fatigue Detection** adalah sistem terintegrasi yang dikembangkan sebagai proyek *internship* di **PT. Anaheim Nimbus Universal**. Sistem ini bertujuan untuk meningkatkan manajemen keamanan dan keselamatan kerja melalui pemantauan berbasis *Computer Vision* secara *real-time*.

Proyek ini memiliki dua fokus utama:
1.  **Crowd Detection:** Memantau kepadatan dan manajemen kerumunan di area tertentu.
2.  **Fatigue Detection:** Mengidentifikasi tanda-tanda kelelahan pada individu untuk mencegah kecelakaan kerja.

---

## 🏗️ Arsitektur Sistem

Berikut adalah gambaran arsitektur sistem yang menghubungkan model Deep Learning, Backend API, dan Frontend Dashboard:

<div align="center">
  <img src="https://github.com/user-attachments/assets/952682a3-83c4-4220-8b8e-705b9ca91955" alt="Arsitektur Sistem Crowd and Fatigue Detection" width="100%">
</div>

---

## 🚀 Fitur Utama

### 1. 👥 Crowd Detection (Manajemen Kerumunan)
Bertujuan untuk mendeteksi, menganalisis, dan memantau kerumunan pada suatu area tertentu.
* **Real-time Counting:** Menghitung jumlah orang dalam area secara langsung.
* **Crowd Analysis:** Memberikan wawasan data untuk manajemen ruang dan keamanan.

### 2. 😴 Fatigue Detection (Deteksi Kelelahan)
Bertujuan mengidentifikasi tanda-tanda kelelahan berdasarkan analisis gerak mata dan mulut. Sistem menggunakan logika ambang batas waktu (*threshold*) sebagai berikut:
* **Menguap (Yawning):** Terdeteksi jika mulut terbuka lebar selama **> 3 detik**.
* **Mengantuk (Drowsiness):** Terdeteksi jika mata tertutup selama **> 4 detik**.

---

## 🛠️ Teknologi yang Digunakan (Tech Stack)

Sistem ini dibangun menggunakan serangkaian teknologi modern untuk memastikan performa yang cepat dan akurat.

| Komponen | Teknologi | Deskripsi |
| :--- | :--- | :--- |
| **Machine Learning** | ![YOLOv11](https://img.shields.io/badge/YOLO-v11-blue?style=flat-square) | Model *Deep Learning* canggih untuk deteksi objek dan analisis fitur wajah yang cepat. |
| **Backend** | ![Express.js](https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white) | Framework server untuk autentikasi, otorisasi, dan manajemen data *real-time*. |
| **Frontend** | ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white) | Dibangun dengan **Vite** dan **Chakra UI** untuk antarmuka yang responsif. Menggunakan **Axios** & **SWR** untuk *data fetching*. |
| **Database** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white) | Database relasional untuk menyimpan data pengguna dan log hasil analisis deteksi. |

---

## 💡 Implementasi & Alur Kerja

Pengembangan proyek ini dilakukan melalui empat tahapan utama:

1.  **AI Model Development:**
    Mengembangkan model menggunakan **YOLOv11** untuk mendeteksi kerumunan dan mengenali kondisi wajah (mata tertutup/mulut menguap) dengan akurasi tinggi.

2.  **Backend Services:**
    Membangun REST API menggunakan **Express.js** yang melayani:
    * Endpoint Autentikasi & Otorisasi (Login/Register).
    * Operasi CRUD (*Create, Read, Update, Delete*).
    * Manajemen pengiriman dan penerimaan data deteksi secara *real-time*.

3.  **Frontend Interface:**
    Membangun dashboard web interaktif menggunakan **React (Vite) + TypeScript**.
    * Desain antarmuka menggunakan **Chakra UI**.
    * Optimasi performa data dengan **SWR** dan **Axios**.

4.  **Database Management:**
    Implementasi **PostgreSQL** untuk menyimpan data pengguna yang terstruktur serta mengarsipkan hasil analisis deteksi dari layanan Crowd dan Fatigue Detection secara terorganisir.

---

<div align="center">
  <small>Developed by Intern Team @ PT. Anaheim Nimbus Universal</small>
</div>
