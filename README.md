# Yüz Tanıma ve Eşleştirme Sistemi (Face Recognition)

Bu proje, Sayısal Görüntü İşleme dersi dönem projesi kapsamında geliştirilmiş, **OpenCV** kütüphanesi kullanılarak görüntü üzerinden yüz algılama ve algılanan yüzlerin sisteme kayıtlı yüzlerle eşleştirilmesini sağlayan bir makine öğrenmesi sistemidir.

<img width="1863" height="902" alt="image" src="https://github.com/user-attachments/assets/0b33615d-d0b3-4dea-86d9-50932a99e501" />


## 📌 Proje Konusu
Projede, OpenCV kütüphanesinde yer alan **HaarCascade** algoritması kullanılarak görüntü üzerinden yüzler algılanmaktadır. Algılanan yüzler, sisteme daha önceden kaydedilmiş yüz verileriyle **LBPH (Local Binary Patterns Histograms)** algoritması kullanılarak karşılaştırılır. Eşleşme sağlanırsa kişinin adı ekranda yeşil bir çerçeve ile gösterilir. Yüz sistemde kayıtlı değilse kullanıcıya kırmızı bir çerçeve ile "Kayitli Degil" mesajı verilir.

## 📂 Klasör Yapısı
Proje, eğitim ve testin yapılabilmesi için aşağıdaki gibi yapılandırılmıştır:

* **`dataset/oyuncu_yuzleri/`**: Modeli eğitmek için kullanılan yüz veri setini içerir (5 farklı sinema oyuncusuna ait 2'şer adet olmak üzere toplam 10 görüntü).
* **`dataset/test_images/`**: Eğitilen modelin başarımını test etmek için kullanılan farklı açılardan yüz görüntüleri.
* **`project.ipynb`**: Yüz algılama, model eğitimi ve test aşamalarını içeren ana Python kod dosyası.
* **`docs/`**: Proje gereksinim dokümanları.

## 🚀 Kullanılan Teknolojiler
* **Python 3**
* **OpenCV** (`haarcascade_frontalface_default.xml`, `cv2.face.LBPHFaceRecognizer_create`)
* **NumPy**
* **Matplotlib** (Sonuçların görselleştirilmesi için)

## ⚙️ Kurulum ve Çalıştırma
1. Bu projeyi indirin.
2. `dataset` klasörünün içindeki verileri Google Drive'ınızda `/MyDrive/FaceProject/` yoluyla erişilebilecek şekilde yükleyin.
3. `project.ipynb` dosyasını **Google Colab** üzerinden açın.
4. İlk hücredeki Drive bağlama işlemini onaylayın ve ardından hücreleri sırasıyla çalıştırın. Test resimleri üzerindeki başarımları ekranınızda görebilirsiniz.
