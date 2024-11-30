# Health Status and Heart Attack Risk: EDA, Regression, and Hypothesis Testing Analysis

![health](https://github.com/user-attachments/assets/3c62c98f-a6f2-4591-9fe9-7a8894c418e7)


Veri setinin boyutu büyük olduğu için githuba eklenememiştir.
- **Veri seti: https://www.kaggle.com/datasets/tarekmuhammed/patients-data-for-medical-field/data**
- **Repo : https://www.kaggle.com/code/lknurylmaz/sa-l-k-durumu-ve-kalp-krizi-riski-eda-regresyon**

  
Veri seti aşağıdaki özellikleri içermektedir:

- **PatientID:** Unique identifier for each patient.
- **State:** Geographic state of residence.
- **Sex:** Gender of the patient.
- **GeneralHealth:** Self-reported health status.
- **AgeCategory:** Categorized age group of the patient.
- **HeightInMeters:** Height of the patient (in meters).
- **WeightInKilograms:** Weight of the patient (in kilograms).
- **BMI:** Body Mass Index, calculated from height and weight.
- **HadHeartAttack:** Indicator of whether the patient had a heart attack.
- **HadAngina:** Indicator of whether the patient experienced angina.
- **HadStroke:** Indicator of whether the patient had a stroke.
- **HadAsthma:** Indicator of whether the patient has asthma.
- **HadSkinCancer:** Indicator of whether the patient had skin cancer.
- **HadCOPD:** Indicator of whether the patient had chronic obstructive pulmonary disease (COPD).
- **HadDepressiveDisorder:** Indicator of whether the patient was diagnosed with a depressive disorder.
- **HadKidneyDisease:** Indicator of whether the patient had kidney disease.
- **HadArthritis:** Indicator of whether the patient had arthritis.
- **HadDiabetes:** Indicator of whether the patient had diabetes.
- **DeafOrHardOfHearing:** Indicator of hearing impairment.
- **BlindOrVisionDifficulty:** Indicator of vision impairment.
- **DifficultyConcentrating:** Indicator of concentration difficulties.
- **DifficultyWalking:** Indicator of walking difficulties.
- **DifficultyDressingBathing:** Indicator of difficulties in dressing or bathing.
- **DifficultyErrands:** Indicator of difficulties in running errands.
- **SmokerStatus:** Status of whether the patient is a smoker.
- **ECigaretteUsage:** Indicator of e-cigarette usage.
- **ChestScan:** Indicator of whether the patient had a chest scan.
- **RaceEthnicityCategory:** Race or ethnicity of the patient.
- **AlcoholDrinkers:** Status of whether the patient consumes alcohol.
- **HIVTesting:** Status of whether the patient was tested for HIV.
- **FluVaxLast12:** Status of whether the patient received a flu vaccine in the last 12 months.
- **PneumoVaxEver:** Status of whether the patient ever received a pneumococcal vaccine.
- **TetanusLast10Tdap:** Status of whether the patient received a tetanus vaccine in the last 10 years.
- **HighRiskLastYear:** Indicator of whether the patient was at high risk in the last year.
- **CovidPos:** Status of whether the patient tested positive for COVID-19.
  
Bu veri seti, kalp hastalığı gibi sonuçları tahmin etmek için çok önemli olan hem tıbbi geçmişi hem de sağlıkla ilgili davranışsal özellikleri içerir. Genel demografik verileri, yaşam tarzı faktörlerini ve belirli sağlık koşullarını içerir. 

## Veri Yükleme ve Ön İşleme

İlk adım olarak, veri seti yüklenmiştir ve eksik değerler, gereksiz sütunlar gibi veriyi etkileyebilecek problemler temizlenmiştir. Bu adımda verinin yapısı gözden geçirilmiş ve sayısal olmayan veriler sayısal verilere dönüştürülmüştür.

## Veri Tiplerinin Seçimi ve Korelasyon Matrisi Hesaplama

Sadece sayısal veriler seçilmiş ve bu veriler arasında korelasyon hesaplanmıştır. Korelasyon matrisi, değişkenler arasındaki ilişkileri anlamamıza yardımcı olur. Özellikle, BMI ve kalp krizi gibi sağlıkla ilgili değişkenler arasındaki olası bağlantılar incelenmiştir.
Korelasyon matrisi görselleştirilmiş ve bu görsel, sayısal özellikler arasındaki güçlü ve zayıf ilişkileri açıkça göstermiştir.

## Keşifsel Veri Analizi (Exploratory Data Analysis - EDA)

EDA aşamasında, veri setinin özelliklerini anlamak için temel istatistikler ve görselleştirmeler kullanılmıştır. Dağılımlar, ortalamalar, medyanlar gibi önemli metrikler hesaplanarak veri üzerinde genel bir analiz yapılmıştır.

##  Hipotez Testi: BMI ve Kalp Krizi İlişkisi
Hipotez testi yapılmıştır: Kalp krizi geçiren ve geçirmeyen kişilerin BMI ortalamaları arasında anlamlı bir fark olup olmadığı test edilmiştir.
Bağımsız İki Örneklem T Testi (t-test) kullanılmıştır. Bu test, iki grup arasındaki ortalama farkının istatistiksel olarak anlamlı olup olmadığını test eder.
T-testinin sonuçları (t-istatistiği ve p-değeri) hesaplanmış ve yorumlanmıştır.

##  Veri Görselleştirme
Boxplot (kutu grafiği) ile kalp krizi geçiren ve geçirmeyen kişilerin BMI değerleri arasındaki fark görselleştirilmiştir. Bu grafik, her iki grubun BMI dağılımlarını göstererek aralarındaki olası farklılıkları görsel olarak ortaya koymuştur.
Boxplot, özellikle gruplar arasındaki medyan, çeyrekler ve uç noktaları görselleştirerek veri hakkında daha fazla bilgi sunar.

# Sonuçların Yorumlanması
Hipotez testinin sonucu ve görselleştirmeler kullanılarak BMI ile kalp krizi arasındaki ilişki değerlendirilmiştir. Eğer test sonucu anlamlı bir fark tespit etmişse, bu, BMI'nin kalp krizi riskiyle ilişkili olabileceği anlamına gelir.

# Model Geliştirme ve Sonuçların Kullanımı
Bu aşamada, kalp krizi riskini tahmin etmek için regresyon modelleri kullanılmıştır. Sonuçlar, sağlık risklerini anlamada ve önleyici tedbirlerin alınmasında kullanılabilir.
