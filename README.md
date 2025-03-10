# yzm212_2425
___________________________________________________________________________________________________________________________________________________________
10.03.2025 - Naive Bayes
  Projede python üzerinde Gaussian Naive Bayes (GNB) modeli için scikit-learn kullanarak ve kullanmayarak oluşturulan iki kod arasındaki farklılıklar gözlemlenmiştir. Veri seti olarak 2000 örnekten oluşan telefon özellikleri ve fiyatlarına dair örnek veri kullanılmıştır. Modellerin accuracy, training time ve prediction time değerleri hesaplanmış ve karmaşıklık matrisi ile görselleştirilmiştir.
  Doğruluk (accuracy) değerinin her iki kodda da 0.7975 olmak üzere stabil ve eşit olduğu görülmüştür. scikit-learn kullanılan kodda training süresinin ortalama 0.002 saniye ve prediction süresinin ortalama 0.001 saniye olduğu, scikit-learn kullanılmayan kodda training süresinin ortalama 0.001 saniye ve prediction süresinin ortalama 0.03 saniye olduğu gözlemlenmiştir.
  scikit-learn kullanıldığında training süresinin daha uzun olması kütüphanenin kullandığı metotta eksik değerleri kontrol etmek için ek işlemler yapması, diğer kodda ise doğrudan training işlemine geçilmesi ile açıklanabilir. Prediction süresinin scikit-learn kullanıldığında çok daha düşük olması ise kütüphanenin test sırasında bellek üzerinde daha optimize yöntemler kullanması şeklinde yorumlanabilir.

  Kaynakça
    https://www.kaggle.com/datasets/iabhishekofficial/mobile-price-classification
    https://www.geeksforgeeks.org/ml-naive-bayes-scratch-implementation-using-python/
    https://github.com/AssemblyAI-Community/Machine-Learning-From-Scratch/tree/main
    
