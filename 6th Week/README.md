# Telco Customer Churn EDA-Feature Engineering Projesi
![alt text](https://miro.medium.com/proxy/1*osC29H34Bw19gqYFc6FWcA@2x.jpeg)
# Özet
Belirli parametrelere bağlı olarak, özellikleri verilen müşterilerin şirketi terk edip etmeme potansiyelini tahmin edebilecek bir Makine Öğrenmesi modelinin eğitilmesi için veri seti hazır hale getirilmiştir. Proje sonunda, bir telekom şirketindeki müşterilerin şirketi terk etmesinde(Churn) etkili olan değişkenler incelenmiştir. Sonrasında kullanılmak üzere belirli bir örüntüye sahip bir müşterinin şirketi terk etme potansiyelinin hesaplanması için uygun hale getilirmiştir.

Bu projeyle birlikte, müşterilere ait metadatalar kullanılarak geliştirilecek müşteri terk tahminleme modeli öncesi, Keşifçi Veri Analizi(Exploratory Data Analysis-EDA) ve Özellik Mühendisliği(Feature Engineering) işlemlerini yapmaktadır. Bu sayede, veri seti modelin eğitilmesi aşaması için hazır hale getirilerek Cat Boost Classifier makine öğrenmesi algoritması kullanılarak test edildi. Projedeki amaç veri ön işleme olduğundan, model metriklerinin optimizasyonları gözardı edildi. Geliştirilen model üzerinde yapılan testlerde %79 Accuracy ve %74 AUC sonuçları elde edilmiştir.

# Veri Seti
https://www.kaggle.com/blastchar/telco-customer-churn

Telco müşteri kaybı verileri, üçüncü çeyrekte Kaliforniya'daki 7043 müşteriye ev telefonu ve İnternet hizmetleri sağlayan hayali bir telekom şirketi hakkında bilgi içerir. Kaggle'da paylaşılan veri setine göre hangi müşterilerin hizmetlerinden ayrıldığını, kaldığını veya hizmete kaydolduğunu gösterir.

Toplamda 21 Değişken, 7043 Gözlemden oluşmakta olup 977.5 KB boyutundadır.

Veri seti üzerindeki değişkenler sırasıyla şöyledir;

**CustomerId:** Müşteri İd’si

**Gender:** Cinsiyet

**SeniorCitizen:** Müşterinin yaşlı olup olmadığı (1, 0)

**Partner:** Müşterinin bir ortağı olup olmadığı (Evet, Hayır)

**Dependents:** Müşterinin bakmakla yükümlü olduğu kişiler olup olmadığı (Evet, Hayır

**tenure:** Müşterinin şirkette kaldığı ay sayısı

**PhoneService:** Müşterinin telefon hizmeti olup olmadığı (Evet, Hayır)

**MultipleLines:** Müşterinin birden fazla hattı olup olmadığı (Evet, Hayır, Telefon hizmeti yok)

**InternetService:** Müşterinin internet servis sağlayıcısı (DSL, Fiber optik, Hayır)

**OnlineSecurity:** Müşterinin çevrimiçi güvenliğinin olup olmadığı (Evet, Hayır, İnternet hizmeti yok)

**OnlineBackup:** Müşterinin online yedeğinin olup olmadığı (Evet, Hayır, İnternet hizmeti yok)

**DeviceProtection:** Müşterinin cihaz korumasına sahip olup olmadığı (Evet, Hayır, İnternet hizmeti yok)

**TechSupport:** Müşterinin teknik destek alıp almadığı (Evet, Hayır, İnternet hizmeti yok)

**StreamingTV:** Müşterinin TV yayını olup olmadığı (Evet, Hayır, İnternet hizmeti yok)

**StreamingMovies:** Müşterinin film akışı olup olmadığı (Evet, Hayır, İnternet hizmeti yok)

**Contract:** Müşterinin sözleşme süresi (Aydan aya, Bir yıl, İki yıl)

**PaperlessBilling:** Müşterinin kağıtsız faturası olup olmadığı (Evet, Hayır)

**PaymentMethod:** Müşterinin ödeme yöntemi (Elektronik çek, Posta çeki, Banka havalesi (otomatik), Kredi kartı (otomatik))

**MonthlyCharges:** Müşteriden aylık olarak tahsil edilen tutar

**TotalCharges:** Müşteriden tahsil edilen toplam tutar

**Churn:** Müşterinin kullanıp kullanmadığı (Evet veya Hayır)
