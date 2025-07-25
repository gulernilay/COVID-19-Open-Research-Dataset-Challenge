# COVID-19 Open Research Dataset Challenge (CORD-19)

Bu proje, COVID-19 ile ilgili bilimsel makalelerin yer aldığı CORD-19 veri seti üzerinde kapsamlı bir keşifçi veri analizi (EDA), aykırı değer analizi ve veri görselleştirme çalışması sunar. Amaç, veri setindeki önemli eğilimleri, eksiklikleri ve öne çıkan noktaları ortaya çıkarmak ve araştırmacılara hızlı bir genel bakış sağlamaktır.

---

## 📂 Proje İçeriği

- **Veri Yükleme ve Temizleme**

  - `metadata.csv` dosyasının yüklenmesi
  - Eksik ve gereksiz sütunların temizlenmesi
  - Temiz veri setinin oluşturulması

- **Keşifçi Veri Analizi (EDA)**

  - Sayısal ve kategorik değişkenlerin istatistiksel özetleri
  - Sütun tipleri, benzersiz değerler, veri dağılımları

- **Eksik Veri Analizi**

  - Eksik veri oranlarının hesaplanması
  - Eksik verilerin görselleştirilmesi (bar plot, matrix plot)

- **Aykırı Değer Analizi**

  - Yayın yılı gibi değişkenlerde aykırı değerlerin tespiti (IQR yöntemi, eşik değerler)
  - Boxplot ve istatistiksel özetlerle aykırı değerlerin sunulması

- **Veri Görselleştirme**
  - Yayın kaynaklarının dağılımı (bar plot)
  - Lisans türlerinin dağılımı (pie chart, bar plot)
  - En çok yayın yapan dergiler (bar plot)
  - Aylık yayın trendleri (line plot, area plot)

---

## 🚀 Nasıl Kullanılır?

1. **Gereksinimler**

   - Python 3.x
   - Gerekli kütüphaneler:
     ```bash
     pip install pandas numpy matplotlib seaborn missingno
     ```

2. **Veri Seti**

   - [CORD-19 metadata.csv](https://www.semanticscholar.org/cord19) dosyasını proje klasörüne ekleyin.

3. **Notebookları Çalıştırma**
   - `main.ipynb` veya `cord-19-data-analysis-project.ipynb` dosyalarını Jupyter Notebook veya VS Code ile açıp adım adım çalıştırabilirsiniz.

---

## 📁 Dosya Açıklamaları

- **main.ipynb**  
  Ana analiz ve görselleştirme adımlarını içerir.

- **cord-19-data-analysis-project.ipynb**  
  Alternatif analizler ve ek grafikler içerir.

- **metadata.csv**  
  CORD-19 veri seti (dışarıdan temin edilmelidir).

---

## 📊 Örnek Grafikler

- Yayın kaynaklarının dağılımı (bar plot)
- Lisans türlerinin dağılımı (pie chart & bar plot)
- En çok yayın yapan dergiler (horizontal bar plot)
- Aylık yayın trendleri (line plot & area plot)
- Yayın yılı dağılımı ve aykırı değerler (boxplot, histogram)

---

## 📌 Notlar

- Veri setinde çok sayıda eksik ve eski tarihli kayıt olabilir. Analizlerde bu durum dikkate alınmıştır.
- Kodlar ve görseller, veri bilimi ve veri analizi öğrenmek isteyenler için açıklamalı olarak hazırlanmıştır.
- Her türlü katkı ve geri bildirim için pull request gönderebilirsiniz.

---

## 🔗 Kaynaklar

- [CORD-19 Dataset - Semantic Scholar](https://www.semanticscholar.org/cord19)
- [CORD-19 Kaggle](https://www.kaggle.com/datasets/allen-institute-for-ai/CORD-19-research-challenge)

---

**Hazırlayan:**  
[Adınızı buraya yazabilirsiniz]
