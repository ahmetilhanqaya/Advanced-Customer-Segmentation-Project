Müşteri Segmentasyonu (K-Prototypes Clustering)
Bu proje, bir müşteri verisetini analiz ederek müşterileri benzer davranış özelliklerine göre gruplandırmayı (segmentasyon) amaçlar.
Makine öğrenmesi dünyasında bu işleme "Unsupervised Learning" (Gözetimsiz Öğrenme) denir.

Proje Özeti
Verisetimizdeki müşterileri; yaş, gelir ve diğer kategorik özelliklerine göre 10 farklı segmente ayırdık.
Bu tür bir çalışma, şirketlerin her müşteri grubuna özel pazarlama stratejileri geliştirmesine yardımcı olur.


Veri Hazırlama ve İşleme
Veri Temizleme: Eksik veriler (null) kontrol edildi ve veri bütünlüğü sağlandı.

Normalizasyon: Gelir ve Yaş gibi farklı ölçeklerdeki veriler, algoritmanın daha sağlıklı çalışması için MinMaxScaler ile 0-1 arasına çekildi.

Özellik Seçimi: Kümeleme işlemine dahil edilmeyecek olan ID sütunu veri setinden çıkarıldı.

Model: K-Prototypes
Neden K-Means yerine K-Prototypes kullandık?

K-Means: Sadece sayısal verilerle (gelir, yaş) çalışabilir.

K-Modes: Sadece kategorik verilerle (meslek, eğitim) çalışabilir.

K-Prototypes: Her iki veri tipini de harmanlayarak gerçek dünya verilerine en uygun sonucu verir.

Görselleştirme
Kümeleme işlemi bittikten sonra, müşterilerin Gelir ve Yaş dağılımları farklı renklerle görselleştirilmiştir.
Bu sayede her bir kümenin (cluster) hangi yaş ve gelir grubuna hitap ettiği net bir şekilde gözlemlenebilmektedir.

Daha Fazla Görselleştirme: Sadece yaş ve gelir değil, eğitim seviyesine göre de dağılım incelenebilir.
