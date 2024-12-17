# Car Price Prediction using Linear Regression

This project develops a **Car Price Prediction Model** using **Linear Regression**. The model predicts the price of a car based on its features such as horsepower, engine size, fuel type, and more.

---

## Dataset
This dataset contains **technical specifications, performance metrics, and prices of various cars**. 
It can be used for Machine Learning tasks such as price prediction, regression analysis, or classification. 

---

## Column Descriptions
1. **car_ID**: Unique ID for each car.  
2. **symboling**: Risk rating (-2 = safest, +3 = most risky).  
3. **CarName**: Name of the car (brand and model).  
4. **fueltype**: Type of fuel used (gas or diesel).  
5. **aspiration**: Engine type (standard or turbo).  
6. **doornumber**: Number of doors (two or four).  
7. **carbody**: Body style of the car (sedan, hatchback, etc.).  
8. **drivewheel**: Type of drive (front, rear, or 4-wheel drive).  
9. **enginelocation**: Location of the engine (front or rear).  
10. **wheelbase**: Distance between the wheel axles (inches).  
11. **carlength**: Length of the car (inches).  
12. **carwidth**: Width of the car (inches).  
13. **carheight**: Height of the car (inches).  
14. **curbweight**: Weight of the car (pounds).  
15. **enginetype**: Type of engine used (ohc, ohcv, etc.).  
16. **cylindernumber**: Number of engine cylinders (two, four, etc.).  
17. **enginesize**: Engine size in cubic centimeters (cc).  
18. **fuelsystem**: Fuel system used (mpfi, spdi, carb, etc.).  
19. **boreratio**: Ratio of the bore diameter to the stroke length.  
20. **stroke**: Piston stroke length.  
21. **compressionratio**: Compression ratio of the engine.  
22. **horsepower**: Horsepower of the engine.  
23. **peakrpm**: Peak revolutions per minute (RPM) of the engine.  
24. **citympg**: Fuel efficiency in city driving (miles per gallon).  
25. **highwaympg**: Fuel efficiency on the highway (miles per gallon).  
26. **price**: Price of the car (in USD). 

---

## **Steps**

1. **Data Loading and Preprocessing**  
   - Null values are checked.  
   - String columns are encoded to numeric representations.

2. **Feature Engineering**  
   - Car brand names are extracted from `CarName`.  
   - Categorical variables are converted using **One-Hot Encoding**.

3. **Model Training and Testing**  
   - The data is split into **Training (80%)** and **Test (20%)** sets.  
   - A **Linear Regression** model is trained on the training set.  

4. **Model Evaluation**  
   - Model performance is measured using:  
     - **Mean Squared Error (MSE)**  
     - **Mean Absolute Error (MAE)**  
     - **R² Score**  

---

## **Results**

The trained Linear Regression model achieves the following results:

| Metric                       | Value         |
|------------------------------|---------------|
| **Mean Squared Error (MSE)** | `8130814.69`  |
| **Mean Absolute Error (MAE)**| `1950.47`     |
| **R² Score**                 | `0.90`        |

### Key Interpretation:  
- An **R² score of 0.90** indicates that **90%** of the variance in car prices is explained by the model.
---
# Lineer Regresyon ile Araba Fiyat Tahmini

Bu proje, **Lineer Regresyon** kullanarak bir **Araba Fiyat Tahmin Modeli** oluşturur. Model, beygir gücü, motor hacmi, yakıt türü gibi özelliklere dayalı olarak araba fiyatlarını tahmin eder.

---

## Veriseti
Bu veri kümesi, **çeşitli otomobillerin teknik özelliklerini, performans ölçümlerini ve fiyatlarını** içermektedir.
Fiyat tahmini, regresyon analizi veya sınıflandırma gibi Makine Öğrenimi projelerinde kullanılabilir.

---

## Sütun Açıklamaları
1. **car_ID**: Her araba için benzersiz kimlik numarası.  
2. **symboling**: Risk derecesi (-2 en güvenli, +3 en riskli).  
3. **CarName**: Arabanın adı (marka ve model).  
4. **fueltype**: Yakıt türü (benzin veya dizel).  
5. **aspiration**: Motor tipi (standart veya turbo).  
6. **doornumber**: Kapı sayısı (iki veya dört).  
7. **carbody**: Arabanın gövde tipi (sedan, hatchback vb.).  
8. **drivewheel**: Çekiş tipi (ön, arka veya dört teker çekiş).  
9. **enginelocation**: Motor konumu (ön veya arka).  
10. **wheelbase**: Tekerlekler arasındaki mesafe (inç cinsinden).  
11. **carlength**: Arabanın uzunluğu (inç).  
12. **carwidth**: Arabanın genişliği (inç).  
13. **carheight**: Arabanın yüksekliği (inç).  
14. **curbweight**: Arabanın ağırlığı (pound).  
15. **enginetype**: Kullanılan motor tipi (ohc, ohcv vb.).  
16. **cylindernumber**: Motor silindir sayısı (iki, dört vb.).  
17. **enginesize**: Motor hacmi (cc cinsinden).  
18. **fuelsystem**: Yakıt sistemi (mpfi, spdi, carb vb.).  
19. **boreratio**: Silindir çapı ve stroku oranı.  
20. **stroke**: Piston stroğu uzunluğu.  
21. **compressionratio**: Motorun sıkıştırma oranı.  
22. **horsepower**: Motorun beygir gücü.  
23. **peakrpm**: Motorun maksimum devri (RPM).  
24. **citympg**: Şehir içi yakıt verimliliği (mil/galon).  
25. **highwaympg**: Şehir dışı yakıt verimliliği (mil/galon).  
26. **price**: Arabanın fiyatı (USD cinsinden).
    
---

## **Adımlar**

1. **Veri Yükleme ve Ön İşleme**  
   - Eksik değerler kontrol edildi.  
   - Metin sütunları sayısal verilere dönüştürüldü.

2. **Özellik Mühendisliği**  
   - `CarName` sütunundan araba markaları ayrıştırıldı.  
   - Kategorik değişkenler **One-Hot Encoding** yöntemiyle dönüştürüldü.

3. **Modelin Eğitilmesi ve Test Edilmesi**  
   - Veriler **%80 Eğitim** ve **%20 Test** şeklinde ayrıldı.  
   - Lineer Regresyon modeli eğitim verileriyle eğitildi.

4. **Modelin Değerlendirilmesi**  
   - Model performansı aşağıdaki metriklerle ölçüldü:  
     - **Ortalama Kare Hatası (MSE)**  
     - **Ortalama Mutlak Hata (MAE)**  
     - **R² Skoru**

---

## **Sonuçlar**

Eğitilmiş Lineer Regresyon modeli aşağıdaki sonuçlara ulaşmıştır:

| Metrik                       | Değer         |
|------------------------------|---------------|
| **Ortalama Kare Hatası (MSE)** | `8130814.69` |
| **Ortalama Mutlak Hata (MAE)**| `1950.47`     |
| **R² Skoru**                 | `0.90`        |

### Yorum:  
- **R² Skoru 0.90**, araba fiyatlarındaki değişimin **%90'ının** modelin girdi özellikleriyle açıklanabildiğini gösterir.

---
