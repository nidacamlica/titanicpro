# titanicpro

İşte Titanic veri seti üzerinde yapılan analiz ve modelleme projeniz için README dosyasının Türkçe bir versiyonu:

Titanic: Felaketten Hayatta Kalma Makine Öğrenmesi
Bu proje, Kaggle’ın Titanic Makine Öğrenmesi: Felaketten Hayatta Kalma yarışmasında kullanılan ünlü Titanic veri setine dayanmaktadır. Projenin amacı, yaş, sınıf, cinsiyet, bilet ücreti gibi çeşitli özellikler kullanılarak bir yolcunun hayatta kalıp kalmayacağını tahmin etmektir. Veri seti, Titanic'teki yolcular hakkında bilgi içerir ve bu analiz, hayatta kalmayı tahmin edebilen bir model oluşturmak için makine öğrenmesi tekniklerini kullanacaktır.

Proje Özeti
Bu projenin amacı, Titanic felaketi üzerine veri analizi ve makine öğrenmesi yaparak, hayatta kalmayı etkileyen faktörleri keşfetmek ve yolcuların özelliklerine dayalı hayatta kalma tahmininde bulunacak bir model oluşturmaktır.

Veri Seti
Titanic veri seti aşağıdaki özellikleri içerir:

Survived: Yolcunun hayatta kalıp kalmadığı (1 = Hayatta kaldı, 0 = Hayatını kaybetti).
Pclass: Yolcunun sınıfı (1, 2, ya da 3).
Name: Yolcunun adı.
Sex: Yolcunun cinsiyeti (erkek veya kadın).
Age: Yolcunun yaşı.
SibSp: Yolcunun kardeşi/eşinin sayısı.
Parch: Yolcunun ebeveyni/çocuklarının sayısı.
Fare: Yolcunun ödediği bilet ücreti.
Embarked: Yolcunun bindiği liman (C = Cherbourg; Q = Queenstown; S = Southampton).
Yapılan Adımlar
1. Keşifsel Veri Analizi (EDA):
Veri seti yüklendi ve incelendi.
Eksik veriler tespit edilip, uygun şekilde işlendi.
Seaborn ve matplotlib kullanarak görselleştirmeler yapıldı. Bar grafikleri, ısı haritaları ve korelasyon matrisleri gibi grafikler oluşturuldu.
2. Veri Ön İşleme:
Eksik veriler (örneğin, Yaş ve Fare için) uygun stratejilerle dolduruldu (Yaş ve Fare için medyan, Embarked için mod).
Kategorik veriler (örneğin, Cinsiyet, Embarked) sayısal verilere dönüştürüldü.
Modelin başarısını artırmak amacıyla yeni özellikler (örneğin, AgeGroup) eklendi.
3. Modelleme:
Veriler eğitim ve test setlerine ayrıldı.
Random Forest Classifier modeli oluşturularak hayatta kalma tahminleri yapıldı.
Model değerlendirilerek doğruluk, karışıklık matrisi, ROC eğrisi ve AUC gibi metrikler kullanıldı.
Modelin sağlamlığını test etmek için çapraz doğrulama (cross-validation) yapıldı.
GridSearchCV ile hiperparametre ayarlaması yapılarak modelin performansı iyileştirildi.
4. Model Değerlendirmesi:
Model, test seti üzerinde değerlendirildi ve hiperparametre ayarlarından önceki ve sonraki performans karşılaştırıldı.
Modelin doğruluğu, hiperparametre ayarlamaları sonrası önemli ölçüde iyileştirildi.
5. Özelliklerin Önem Derecesi:
Farklı özelliklerin model üzerindeki etkilerini görmek için özelliklerin önem dereceleri görselleştirildi.
6. Hayatta Kalma Oranı:
Veri setindeki genel hayatta kalma oranı hesaplanarak, veri hakkında daha fazla bilgi edinildi.
Model Sonuçları
Son Model Doğruluğu: [Buraya son doğruluk skorunuzu yazın]
AUC: [Buraya son AUC skorunuzu yazın]
Sonuç
Bu proje, Titanic'teki hayatta kalma durumunu tahmin etmek için bir makine öğrenmesi modeli oluşturma sürecini göstermektedir. Keşifsel veri analizi, veri ön işleme ve model değerlendirme adımlarıyla, doğru sonuçlar veren bir Random Forest Classifier modeli oluşturulmuştur
