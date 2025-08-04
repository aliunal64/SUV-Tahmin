🚀 SUV Satın Alma Tahmini Projesi: Karar Ağacı Yöntemi

🎯 Projenin Amacı

Bu projenin temel amacı, bir veri setini kullanarak tahmin yeteneği olan bir model geliştirmektir.Bu çalışmada;

🧠 Veriden anlamlı sonuçlar çıkararak potansiyel müşteri davranışlarını öngörebilen bir sistemin nasıl kurulduğu gösterilmektedir.

👥💳 Bir kişinin demografik ve finansal bilgilerine dayanarak, bir SUV satın alıp almayacağını tahmin eden bir model oluşturulmuştur.

🧮 Sınıflandırma görevini gerçekleştirmek için Karar Ağacı (Decision Tree) algoritması kullanılmıştır.

------------------------------------------------------------------------

🔍 Proje Adımları

Proje kapsamında aşağıdaki adımlar detaylı bir şekilde ele alınmıştır:

📊 Veri setini analiz ederek tahmin için uygun hale getirme.

🌳 Karar Ağacı algoritmasını bir sınıflandırma modeline uygulama.

✅ Geliştirilen modelin performansını ölçerek ne kadar güvenilir olduğunu değerlendirme.

------------------------------------------------------------------------

📚 Kullanılan Veri Seti

Bu projede, Kaggle platformundan elde edilen ve 400 müşterinin bilgilerini içeren suv_data.csv dosyası kullanılmıştır.

Veri setinin sütunları ve içerikleri şunlardır:

👤 User ID: Her bir müşteriye ait benzersiz kimlik numarası.

🚻 Gender: Müşterinin cinsiyet bilgisi.

🎂 Age: Müşterinin yaşı.

💰 EstimatedSalary: Müşterinin tahmini yıllık geliri.

🛒 Purchased: Hedef Değişken. SUV satın alınıp alınmadığını gösteren ikili değer (0: Hayır, 1: Evet).

------------------------------------------------------------------------

🛠️ Uygulanan Yöntemler ve Adımlar

Proje, makine öğrenimi projelerinin standart bir iş akışını takip ederek geliştirilmiştir.

1️⃣ Veri Ön İşleme ⚙️

📂 Veri Yükleme: pandas kütüphanesi ile veri seti bir DataFrame'e yüklenmiştir.

🧹 Veri Keşfi: .shape, .info(), .describe() komutlarıyla veri seti incelenmiştir.

🗑️ Veri Temizleme: User ID sütunu çıkarılmıştır.

🏷️ Kategorik Veri Dönüşümü: Gender sütunu LabelEncoder ile sayısallaştırılmıştır.

✂️ Veri Bölme: Özellikler (X) ve hedef değişken (y) olarak ayrılmış, 
ardından %75 / %25 oranıyla train_test_split yapılmıştır.

------------------------------------------------------------------------

2️⃣ Model Geliştirme ve Tahmin 🤖

🌲 Model Seçimi: sklearn.tree kütüphanesinden Karar Ağacı modeli seçilmiştir.

🎓 Eğitim: Model, X_train ve y_train ile eğitilmiştir.

🔮 Tahmin: X_test verisiyle tahminler yapılmıştır.

------------------------------------------------------------------------

3️⃣ Model Değerlendirme ✅

📉 Modelin performansı çeşitli metriklerle değerlendirilmiştir.

📊 Karmaşıklık Matrisi (Confusion Matrix) oluşturulmuştur.

🎯 Doğruluk Skoru (Accuracy Score) hesaplanmıştır.

------------------------------------------------------------------------

💡 Sonuç ve Çıkarımlar

Bu proje, Karar Ağacı algoritmasının sınıflandırma problemlerinde nasıl etkili şekilde kullanılabileceğini göstermektedir.
Yapılan analizler sonucunda; yaş ve tahmini maaş gibi değişkenlerin, bir kişinin SUV satın alma kararı üzerinde güçlü etkileri olduğu gözlemlenmiştir.
