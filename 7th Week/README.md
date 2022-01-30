# Lineer Regresyon ile Hitters Salary Prediction Çalışması
<p align="center">
  <img src="https://www.parkgrandlondon.co.uk/blog/wp-content/uploads/2019/05/Baseball-in-London.jpg">  
</p>
  
<p align="center">
  <i>Fotoğraf: www.parkgrandlondon.co.uk<i/> 
</p>

# Özet
Bu çalışmada, maaş bilgileri ve 1986 yılına ait kariyer istatistikleri paylaşılan beyzbol oyuncularının verileri Lineer Regresyon tekniği kullanılarak maaş tahminlemesi yapılmıştır. Çalışma sonunda elde edilen model sayesinde, belirli parametreleri verilen bir oyuncunun maaş tahmini %75 başarı oranında tahmin edilebilmiştir. 
  
Çalışma sonunda elde edilen oyuncu maaş tahmini modeli öncesinde, veri setinin doğru bir şekilde yorumlanabilmesi ve işlenebilmesi için Keşifçi Veri Analizi(Exploratory Data Analysis-EDA) ve Özellik Mühendisliği(Feature Engineering) işlemleri yapılmıştır. Çalışma süresince izlenen işlem basamakları sırasıyla şu şekildedir;
 * Exploratory Data Analysis (Keşifçi Veri Analizi)
 * Korelasyon Analizi
 * Feature Engineering (Özellik Mühendisliği)
 * Feature Extraction (Değişken Türetme)
 * Encoding (Kodlama)
 * Model Oluşturma 
 * Tahminleme
 * Tahminleme Başarı Testi
 
# Veri Seti
https://www.kaggle.com/floser/hitters
  
Bu veri seti orijinal olarak Carnegie Mellon Üniversitesi'nde bulunan StatLib kütüphanesinden alınmıştır. Veri seti 1988 ASA Grafik Bölümü Poster Oturumu'nda kullanılan verilerin bir parçasıdır. Maaş verileri orijinal olarak Sports Illustrated, 20 Nisan 1987'den alınmıştır. 1986 ve kariyer istatistikleri, Collier Books, Macmillan Publishing Company, New
York tarafından yayınlanan 1987 Beyzbol Ansiklopedisi Güncellemesinden elde edilmiştir. Şuanda da Kaggle üzerinden paylaşılmaktadır. 
  
Toplamda 20 Değişken, 6440 Gözlemden oluşmakta olup 20.91 KB boyutundadır.

Veri seti üzerindeki değişkenler sırasıyla şöyledir;
  
**AtBat:** 1986-1987 sezonunda bir beyzbol sopası ile topa yapılan vuruş sayısı
  
**Hits:** 1986-1987 sezonundaki isabet sayısı
  
**HmRun:** 1986-1987 sezonundaki en değerli vuruş sayısı
  
**Runs:** 1986-1987 sezonunda takımına kazandırdığı sayı
  
**RBI:** Bir vurucunun vuruş yaptıgında koşu yaptırdığı oyuncu sayısı
  
**Walks:** Karşı oyuncuya yaptırılan hata sayısı
  
**Years:** Oyuncunun major liginde oynama süresi (sene)
  
**CAtBat:** Oyuncunun kariyeri boyunca topa vurma sayısı
  
**CHits:** Oyuncunun kariyeri boyunca yaptığı isabetli vuruş sayısı
  
**CHmRun:** Oyucunun kariyeri boyunca yaptığı en değerli sayısı
  
**CRuns:** Oyuncunun kariyeri boyunca takımına kazandırdığı sayı
  
**CRBI:** Oyuncunun kariyeri boyunca koşu yaptırdırdığı oyuncu sayısı
  
**CWalks:** Oyuncun kariyeri boyunca karşı oyuncuya yaptırdığı hata sayısı
  
**League:** Oyuncunun sezon sonuna kadar oynadığı ligi gösteren A ve N seviyelerine sahip bir faktör
  
**Division:** 1986 sonunda oyuncunun oynadığı pozisyonu gösteren E ve W seviyelerine sahip bir faktör
  
**PutOuts:** Oyun icinde takım arkadaşınla yardımlaşma
  
**Assits:** 1986-1987 sezonunda oyuncunun yaptığı asist sayısı
  
**Errors:** 1986-1987 sezonundaki oyuncunun hata sayısı
  
**Salary:** Oyuncunun 1986-1987 sezonunda aldığı maaş(bin uzerinden)
  
**NewLeague:** 1987 sezonunun başında oyuncunun ligini gösteren A ve N seviyelerine sahip bir faktör

  

  
