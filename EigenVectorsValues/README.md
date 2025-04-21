Makine öğrenmesinde veriler sıklıkla çok boyutlu diziler halinde gelir, bu nedenle matrisler bu tür girdileri işlemek için optimaldir. Makine öğrenmesi algoritmalarını anlamak adına matrislerdeki temel aritmetik işlemler hakkında genel bir fikre sahip olmamız beklenir.

Matris manipülasyonu; matrislerin toplanması, çarpılması, transpozu alınması, tersinin bulunması gibi işlemleri kapsar. Bu bağlamda, özdeğer ve özvektör kavramları matris manipülasyon işlemlerinde önemli bir yere sahiptir. Bir kare matris A için sıfırdan farklı bir vektör v ve bir skaler lambda olmak üzere Av=λv eşitliğini sağlayan tüm v vektörlerine A’nın özvektörü, tüm lambda skaler değerlerine ise A’nın özdeğeri adı verilir. Özdeğerler ve özvektörler, bir matrisin karakteristiğini belirlemede, özellikle de matrisin nasıl bir dönüşüm uyguladığını anlamak için gereklidir. 

Temel Bileşenler Analizi (PCA), Tekil Değer Ayrışımı (SVD) gibi makine öğrenmesi algoritmaları veri matrislerini belirli bir anlamda basitleştirme veya dönüştürmek amacıyla matrislerin özdeğer ve özvektör analizlerinden yararlanır. Bu tür analizler, yüksek boyutlu verilerde en önemli bilgiyi koruyarak boyut indirgeme veya verinin temel yapısını ortaya çıkarma gibi hedefler doğrultusunda kullanılır.

NumPy'nin linalg.eig fonksiyonu, bir kare matrisin özdeğerlerini ve bu özdeğerlere karşılık gelen özvektörlerini bulmak için kullanılır. Fonksiyon çalışırken önce verilen matris uygun bir düzene sokulur ve arka planda LAPACK kütüphanesine ait geev fonksiyonu kullanılır. Bu işlem sırasında matrisin daha basit bir şekil olan üçgensel forma dönüştürülmesi sağlanır, matris üzerinde Schur ayrışımı ve QR yöntemi gibi işlemler uygulayarak özdeğerleri ve özvektörleri bulur. Sonuç olarak, hesaplanan özdeğerler ve özvektörler kullanıcıya NumPy dizileri olarak döndürülür. Eğer matris özel bir yapıya sahipse, örneğin simetrikse, daha doğru sonuçlar almak için eigh isimli başka bir fonksiyonun kullanılması önerilir.

Kaynakça: https://www.geeksforgeeks.org/matrices-and-matrix-arithmetic-for-machine-learning/
https://machinelearningmastery.com/introduction-to-eigendecomposition-eigenvalues-and-eigenvectors/
https://github.com/LucasBN/Eigenvalues-and-Eigenvectors
https://numpy.org/doc/2.1/reference/generated/numpy.linalg.eigh.html



