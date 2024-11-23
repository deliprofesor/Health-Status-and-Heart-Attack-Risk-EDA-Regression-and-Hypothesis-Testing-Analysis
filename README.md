# Health Status and Heart Attack Risk: EDA, Regression, and Hypothesis Testing Analysis

Veri setinin boyutu büyük olduğu için githuba eklenememiştir.
Veri seti: https://www.kaggle.com/datasets/tarekmuhammed/patients-data-for-medical-field/data
Veri seti aşağıdaki özellikleri içermektedir:

PatientID : Her hasta için benzersiz tanımlayıcı.
Eyalet : İkamet edilen coğrafi eyalet.
Cinsiyet : Hastanın cinsiyeti.
GenelSağlık : Kendi bildirilen sağlık durumu.
AgeCategory : Hastanın kategorize edilmiş yaş grubu.
HeightInMeters : Hastanın boyu (metre cinsinden).
WeightInKilograms : Hastanın ağırlığı (kilogram cinsinden).
BMI : Boy ve kilo üzerinden hesaplanan Vücut Kitle İndeksi.
Kalp Krizi Geçirdi : Hastanın kalp krizi geçirip geçirmediğinin göstergesi.
HadAngina : Hastanın angina yaşayıp yaşamadığının göstergesi.
HadStroke : Hastanın inme geçirip geçirmediğinin göstergesi.
HadAsthma : Hastanın astım hastası olup olmadığının göstergesi.
HadSkinCancer : Hastanın cilt kanseri olup olmadığının göstergesi.
KOAH Hastalığı : Hastanın kronik obstrüktif akciğer hastalığı (KOAH) olup olmadığının göstergesi.
HadDepressiveDisorder : Hastanın depresif bozukluk tanısı alıp almadığının göstergesi.
Böbrek Hastalığı Vardı : Hastanın böbrek hastalığı olup olmadığının göstergesi.
Artrit Hastalığı : Hastanın artrit olup olmadığının göstergesidir.
HadDiabetes : Hastanın diyabet hastası olup olmadığının göstergesi.
DeafOrHardOfHearing : İşitme kaybının göstergesi.
BlindOrVisionDifficulty : Görme bozukluğunun göstergesi.
Konsantrasyon Güçlüğü : Konsantrasyon güçlüğünün göstergesi.
Yürüme Zorluğu : Yürüme zorluğunun göstergesi.
Giyinmede veya banyo yapmada zorluk : Giyinme veya banyo yapmada zorluk göstergesi.
DifficultyErrands : İşlerin yapılmasında yaşanan zorlukların göstergesi.
SmokerStatus : Hastanın sigara içip içmediği durumu.
ECigaretteUsage : E-sigara kullanımının göstergesi.
Göğüs Taraması : Hastanın göğüs taraması yapılıp yapılmadığının göstergesi.
IrkEtnik kökenKategori : Hastanın ırkı veya etnik kökeni.
Alkol İçenler : Hastanın alkol tüketip tüketmediği durumu.
HIV Testi : Hastanın HIV testi yaptırıp yaptırmadığı durumu.
FluVaxLast12 : Hastanın son 12 ay içerisinde grip aşısı olup olmadığı durumu.
PneumoVaxEver : Hastanın daha önce pnömokok aşısı olup olmadığı durumu.
TetanusLast10Tdap : Hastanın son 10 yıl içerisinde tetanos aşısı yaptırıp yaptırmadığı durumu.
HighRiskLastYear : Hastanın son bir yılda yüksek risk altında olup olmadığının göstergesi.
CovidPos : Hastanın COVID-19 testinin pozitif olup olmadığı durumu.
Bu veri seti, kalp hastalığı gibi sonuçları tahmin etmek için çok önemli olan hem tıbbi geçmişi hem de sağlıkla ilgili davranışsal özellikleri içerir. Genel demografik verileri, yaşam tarzı faktörlerini ve belirli sağlık koşullarını içerir. 

# Veri Yükleme ve Ön İşleme
İlk adım olarak, veri seti yüklenmiştir ve eksik değerler, gereksiz sütunlar gibi veriyi etkileyebilecek problemler temizlenmiştir. Bu adımda verinin yapısı gözden geçirilmiş ve sayısal olmayan veriler sayısal verilere dönüştürülmüştür.

# Veri Tiplerinin Seçimi ve Korelasyon Matrisi Hesaplama
Sadece sayısal veriler seçilmiş ve bu veriler arasında korelasyon hesaplanmıştır. Korelasyon matrisi, değişkenler arasındaki ilişkileri anlamamıza yardımcı olur. Özellikle, BMI ve kalp krizi gibi sağlıkla ilgili değişkenler arasındaki olası bağlantılar incelenmiştir.
Korelasyon matrisi görselleştirilmiş ve bu görsel, sayısal özellikler arasındaki güçlü ve zayıf ilişkileri açıkça göstermiştir.

# Keşifsel Veri Analizi (Exploratory Data Analysis - EDA)
EDA aşamasında, veri setinin özelliklerini anlamak için temel istatistikler ve görselleştirmeler kullanılmıştır. Dağılımlar, ortalamalar, medyanlar gibi önemli metrikler hesaplanarak veri üzerinde genel bir analiz yapılmıştır.

# Hipotez Testi: BMI ve Kalp Krizi İlişkisi
Hipotez testi yapılmıştır: Kalp krizi geçiren ve geçirmeyen kişilerin BMI ortalamaları arasında anlamlı bir fark olup olmadığı test edilmiştir.
Bağımsız İki Örneklem T Testi (t-test) kullanılmıştır. Bu test, iki grup arasındaki ortalama farkının istatistiksel olarak anlamlı olup olmadığını test eder.
T-testinin sonuçları (t-istatistiği ve p-değeri) hesaplanmış ve yorumlanmıştır.

# Veri Görselleştirme
Boxplot (kutu grafiği) ile kalp krizi geçiren ve geçirmeyen kişilerin BMI değerleri arasındaki fark görselleştirilmiştir. Bu grafik, her iki grubun BMI dağılımlarını göstererek aralarındaki olası farklılıkları görsel olarak ortaya koymuştur.
Boxplot, özellikle gruplar arasındaki medyan, çeyrekler ve uç noktaları görselleştirerek veri hakkında daha fazla bilgi sunar.

# Sonuçların Yorumlanması
Hipotez testinin sonucu ve görselleştirmeler kullanılarak BMI ile kalp krizi arasındaki ilişki değerlendirilmiştir. Eğer test sonucu anlamlı bir fark tespit etmişse, bu, BMI'nin kalp krizi riskiyle ilişkili olabileceği anlamına gelir.

# Model Geliştirme ve Sonuçların Kullanımı
Bu aşamada, kalp krizi riskini tahmin etmek için regresyon modelleri kullanılmıştır. Sonuçlar, sağlık risklerini anlamada ve önleyici tedbirlerin alınmasında kullanılabilir.
