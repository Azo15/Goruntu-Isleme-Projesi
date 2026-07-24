# 👤 Yüz Tanıma ve Eşleştirme Sistemi / Face Recognition & Matching System

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green.svg)](https://opencv.org/)

---

## 🇹🇷 Türkçe

Bu proje, **OpenCV** kütüphanesi kullanılarak görüntü üzerinden yüz algılama ve algılanan yüzlerin sisteme kayıtlı yüzlerle eşleştirilmesini sağlayan bir makine öğrenmesi sistemidir.

<img width="1863" height="902" alt="Application Screenshot" src="https://github.com/user-attachments/assets/0b33615d-d0b3-4dea-86d9-50932a99e501" />

### 📌 Proje Konusu
Projede, OpenCV kütüphanesinde yer alan **HaarCascade** algoritması kullanılarak görüntü üzerinden yüzler algılanmaktadır. Algılanan yüzler, sisteme daha önceden kaydedilmiş yüz verileriyle **LBPH (Local Binary Patterns Histograms)** algoritması kullanılarak karşılaştırılır. 

* **Eşleşme Sağlanırsa:** Kişinin adı ekranda yeşil bir çerçeve ile gösterilir.
* **Kayıtlı Değilse:** Kullanıcıya kırmızı bir çerçeve ile *"Kayitli Degil"* mesajı verilir.

### 📂 Klasör Yapısı
* **`dataset/oyuncu_yuzleri/`**: Modeli eğitmek için kullanılan yüz veri seti (5 farklı kişiye ait toplam 10 görüntü).
* **`dataset/test_images/`**: Eğitilen modelin başarımını test etmek için kullanılan farklı açılardan yüz görüntüleri.
* **`project.ipynb`**: Yüz algılama, model eğitimi ve test aşamalarını içeren ana Jupyter / Colab dosyası.
* **`docs/`**: Proje gereksinim dokümanları.

### 🚀 Kullanılan Teknolojiler
* **Python 3**
* **OpenCV** (`haarcascade_frontalface_default.xml`, `LBPHFaceRecognizer`)
* **NumPy**
* **Matplotlib**

### ⚙️ Kurulum ve Çalıştırma
1. Bu depoyu klonlayın veya indirin:
   ```bash
   git clone [https://github.com/Azo15/OpenCV-Image-Processing-Project.git](https://github.com/Azo15/OpenCV-Image-Processing-Project.git)
