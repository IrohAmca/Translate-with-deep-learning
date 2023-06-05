# Translate-with-deep-learning
Derin öğrenme ve word2vec kullanarak, encoder ve decoder olan iki modül ile türkçe ingilizce makine çevirisi
Model üzerinde kullanılan eğitim veri setleri bu bölümde link olarak verilmiştir.

Encodera verilen ingilizce kelimeler önce kullanım sıkılığına göre tokenizer işleminden geçer daha sonra glove vectörü üzerinden daha önceden belirlenmiş vectörler ile uygun vectörlere dönüştürülür.
Burda kullanılan glove vectörü ingilizce kelimeler için çok geniş bir değer aralığına ve kelime dağarcığına sahip olduğu için bu veriler kullanılımıştır.
Dönüştürülen vectörler decoder ile daha önceden yapılmış eğitim den belirlenen parametreler yardımı ile uygun tokenlere çevrilir.
Son işlem olarak translate fonksiyonu ise bulunan token değerleri daha önceden tokenizer işleminden belirlenmiş kelime değerlerine dönüştürülür.

Glove link:https://www.kaggle.com/datasets/danielwillgeorge/glove6b100dtxt
tur.text link:https://www.kaggle.com/datasets/bulentsiyah/turkce/code
