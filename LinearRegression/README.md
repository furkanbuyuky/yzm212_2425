Bu çalışmada, öğrencilerin günlük çalışma saatleri ile aldıkları başarı skorları arasındaki doğrusal ilişki iki farklı yöntemle modellenmiş ve elde edilen sonuçlar karşılaştırılmıştır. Birinci yöntemde manuel olarak geliştirilmiş bir gradyan iniş algoritması, ikinci yöntemde ise scikit-learn kütüphanesinin sunduğu analitik çözüm kullanılmıştır. Her iki yöntem de ortalama kare hata değerleri üzerinden performans açısından değerlendirilmiştir.

Deneyde kullanılan veri seti, her satırda bir öğrencinin günlük çalışma süresi ve buna karşılık gelen sınav skorunu içerir. Manuel yaklaşımda, başlangıçta eğim ve kesim değerleri sıfır olarak tanımlanmış; daha sonra her iterasyonda, çalışma saati ve skor arasındaki hata bilgisi kullanılarak bu iki parametre güncellenmiştir. Güncelleme adımlarında sabit bir öğrenme oranı seçilmiş ve toplamda bin kez yinelenmiştir.

Scikit-learn kullanan yöntem ise, veri matrisi ve skor vektörü üzerinde kapalı form matematiksel çözümü uygular. Bu sayede tek adımda en küçük kareler ölçütünü tam olarak karşılayan eğim ve kesim değerleri elde edilir. Burada herhangi bir iterasyon sayısı veya öğrenme oranı belirlemeye gerek kalmaz. Model eğitildikten sonra yine ortalama kare hata değeri hesaplanarak performans ölçülmüştür.

Elde edilen sonuçlar şunlardır. Manuel gradyan iniş yönteminde eğim yaklaşık 9,61, kesim yaklaşık 1,06 ve ortalama kare hata değeri 29,06 olarak bulunmuştur. Scikit-learn yöntemi ile elde edilen eğim yaklaşık 9,78, kesim yaklaşık 2,48 ve ortalama kare hata değeri 28,88’dir. Görüldüğü gibi analitik çözüm, manuel yönteme kıyasla daha düşük bir hata değeri sunmaktadır.

Bu farkın nedeni, manuel gradyan iniş algoritmasının sınırlı sayıda iterasyon ve sabit öğrenme oranı ile tam optimum noktaya ulaşamamasıdır. Oysa scikit-learn’ün analitik yöntemi bir yandan normal denklem yaklaşımını bir yandan da sayısal olarak kararlı tekil değer ayrışımı yöntemini kullanarak tamamen en küçük kareler ölçütünü karşılayan sonucu doğrudan üretir. Manuel yöntemin analitik çözüme yaklaşabilmesi için iterasyon sayısının artırılması, öğrenme oranının ayarlanması veya adaptif optimizasyon tekniklerinin tercih edilmesi mümkündür.

Sonuç olarak, basit doğrusal regresyon problemlerinde analitik yöntemler, her koşulda en düşük hatayı elde etmek adına daha güvenilir ve hızlıdır. Bununla birlikte hesaplama kaynakları ve uygulama gereksinimleri izin veriyorsa, uygun hiperparametre seçimi ile manuel gradyan iniş de kabul edilebilir sonuçlar verebilir. Gelecekteki çalışmalarda, farklı düzenlileştirme terimleri ve optimizasyon stratejileri ile modelin genelleme yeteneği üzerine ek deneyler yapılması önerilir.

Kaynakça: https://www.geeksforgeeks.org/linear-regression-python-implementation/ 

https://www.youtube.com/watch?v=VmbA0pi2cRQ
