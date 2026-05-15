# 🏢 AI-Powered Employee Churn Prediction (Çalışan Kaybı Tahmini)

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-0.24+-orange.svg)
![Pandas](https://img.shields.io/badge/Pandas-1.2+-green.svg)

## 📌 Proje Amacı
Bu proje, bir şirketteki çalışanların demografik, davranışsal ve operasyonel verilerini (maaş, çalışma saati, memnuniyet vb.) analiz ederek **istifa etme (churn) olasılıklarını** makine öğrenmesi algoritmalarıyla önceden tahmin etmeyi amaçlar. Şirketlerin yetenek kaybını ve yeniden işe alım (onboarding) maliyetlerini düşürmek için proaktif bir **Erken Uyarı Sistemi** olarak tasarlanmıştır.

## 📊 Veri Seti
Kullanılan veri seti 14.999 satırdan oluşmakta olup, çalışanların;
* Memnuniyet seviyeleri
* Aylık ortalama çalışma saatleri
* Tamamladıkları proje sayıları
* Son 5 yıldaki terfi durumları
* Maaş kategorileri gibi öznitelikleri içermektedir.

## 🧠 Kullanılan Modeller ve Başarı Oranları (Accuracy)
Model performansları, veri setinin eğitimde hiç kullanılmayan %20'lik test bölümü üzerinde ölçülmüştür:
1. **Random Forest:** `% 98.8` 🏆 (En başarılı model)
2. **K-Nearest Neighbors (KNN):** `% 95.3`
3. **Logistic Regression:** `% 75.8`

## 📈 Model Değerlendirmesi
Geleneksel bir model olan *Logistic Regression*, insan davranışları gibi doğrusal olmayan (non-linear) karmaşık verilerde zayıf kalırken; topluluk (ensemble) tabanlı *Random Forest* modeli çalışan kaybını tespit etmede kusursuz bir performans sergilemiştir. 

**ROC ve AUC Skoru:** Random Forest modelinin AUC skoru **0.9910** olarak ölçülmüştür. Bu durum, modelin ayrılacak bir çalışanla kalacak bir çalışanı %99'un üzerinde bir kesinlikle ayırt edebildiğini kanıtlar (Overfitting/Ezberleme yapılmadığı bağımsız test seti ile doğrulanmıştır).

## 🚀 Kurulum ve Kullanım
Bu projeyi kendi lokalinizde çalıştırmak için:
1. Repoyu klonlayın: `git clone https://github.com/KULLANICI_ADIN/HR-Churn-Prediction.git`
2. Jupyter Notebook veya Google Colab üzerinden `HR_Churn_Analysis.ipynb` dosyasını açın.
3. Hücreleri sırayla çalıştırarak matrisleri ve güncel tahminleri görüntüleyin.
