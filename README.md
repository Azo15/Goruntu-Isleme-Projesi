# 👤 Yüz Tanıma ve Eşleştirme Sistemi / Face Recognition & Matching System

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 🇹🇷 Türkçe

Bu proje, Sayısal Görüntü İşleme dersi dönem projesi kapsamında geliştirilmiş, **OpenCV** kütüphanesi kullanılarak görüntü üzerinden yüz algılama ve algılanan yüzlerin sisteme kayıtlı yüzlerle eşleştirilmesini sağlayan bir makine öğrenmesi sistemidir.

<img width="1863" height="902" alt="Application Screenshot" src="https://github.com/user-attachments/assets/0b33615d-d0b3-4dea-86d9-50932a99e501" />

### 📌 Proje Konusu
Projede, OpenCV kütüphanesinde yer alan **HaarCascade** algoritması kullanılarak görüntü üzerinden yüzler algılanmaktadır. Algılanan yüzler, sisteme daha önceden kaydedilmiş yüz verileriyle **LBPH (Local Binary Patterns Histograms)** algoritması kullanılarak karşılaştırılır. 

* **Eşleşme Sağlanırsa:** Kişinin adı ekranda yeşil bir çerçeve ile gösterilir.
* **Kayıtlı Değilse:** Kullanıcıya kırmızı bir çerçeve ile *"Kayitli Degil"* mesajı verilir.

### 📂 Klasör Yapısı
* **`dataset/oyuncu_yuzleri/`**: Modeli eğitmek için kullanılan yüz veri seti (5 farklı sinema oyuncusuna ait 2'şer adet olmak üzere toplam 10 görüntü).
* **`dataset/test_images/`**: Eğitilen modelin başarımını test etmek için kullanılan farklı açılardan yüz görüntüleri.
* **`project.ipynb`**: Yüz algılama, model eğitimi ve test aşamalarını içeren ana Python kod dosyası.
* **`docs/`**: Proje gereksinim dokümanları.

### 🚀 Kullanılan Teknolojiler
* **Python 3**
* **OpenCV** (`haarcascade_frontalface_default.xml`, `cv2.face.LBPHFaceRecognizer_create`)
* **NumPy**
* **Matplotlib**

### ⚙️ Kurulum ve Çalıştırma
1. Bu projeyi indirin.
2. `dataset` klasörünün içindeki verileri Google Drive'ınızda `/MyDrive/FaceProject/` yoluyla erişilebilecek şekilde yükleyin.
3. `project.ipynb` dosyasını **Google Colab** üzerinden açın.
4. İlk hücredeki Drive bağlama işlemini onaylayın ve ardından hücreleri sırasıyla çalıştırın.

---

## 🇬🇧 English

This project was developed as part of a Digital Image Processing course. It is a machine learning system built using **OpenCV** that performs face detection on images and matches detected faces with registered individuals in the database.

### 📌 Overview
The system utilizes the **HaarCascade** algorithm for face detection and the **LBPH (Local Binary Patterns Histograms)** algorithm for face recognition/matching.

* **Recognized Face:** Displayed with a green bounding box and the person's name.
* **Unrecognized Face:** Displayed with a red bounding box and a *"Kayitli Degil"* (Not Registered) message.

### 📂 Directory Structure
* **`dataset/oyuncu_yuzleri/`**: Training dataset containing face images (10 images total for 5 individuals).
* **`dataset/test_images/`**: Test images used to evaluate model performance.
* **`project.ipynb`**: Main Jupyter/Colab notebook containing face detection, training, and testing pipelines.
* **`docs/`**: Project documentation files.

### ⚙️ Installation & Usage
1. Download or clone this repository.
2. Upload the contents of the `dataset` folder to your Google Drive under `/MyDrive/FaceProject/`.
3. Open `project.ipynb` in **Google Colab**.
4. Run the cells sequentially after granting Google Drive access permissions.

---

