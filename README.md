
 🛒 Marketing Insights for E-Commerce
 📊 Layihə Haqqında

Bu layihə, e-commerce şirkətinin satış, müştəri davranışı və marketinq xərcləri üzərində aparılmış SQL əsaslı analitik tədqiqatdır.PostgreSQL istifadə edilərək tranzaksiya səviyyəsində təhlil aparılmış, müştəri segmentasiyası, satış tendensiyaları və gəlir mənbələri müəyyən edilmişdir.

Məqsəd:

1 Satış və gəlir performansını izləmək
2 Müştəri segmentasiyasını müəyyənləşdirmək
3 Marketinq xərclərinin effektivliyini ölçmək
4 Məhsul və kateqoriyalara görə satış trendini anlamaq

🧩 Datasetlər

| Dataset                 | Təsviri                                                                        |
| ----------------------- | ------------------------------------------------------------------------------ |
| Customers_Data.csv      | Müştərilərin demoqrafik məlumatları (ID, Gender, Location, Tenure)             |
| Online_Sales.csv        | Tranzaksiya məlumatları (ID, Date, Product, Quantity, Price, Delivery, Coupon) |
| Discount_Coupon.csv     | Endirim kuponları (Ay, Məhsul Kateqoriyası, Kupon Kodu, Faiz)                  |
| Marketing_Spend.csv     | Offline & online marketinq xərcləri                                            |
|Tax_Amount.csv           | GST faizləri kateqoriyalara görə                                               |

 🔹 Key Insights
1️⃣ Satış və Gəlir Analizi

Aylıq və kateqoriyalara görə satış və gəlir izlənildi.
Ən çox gəlir gətirən məhsullar və kateqoriyalar müəyyən edildi.
Endirimlərin gəlirə təsiri analiz edildi.
Satışlar müəyyən aylarda və xüsusi günlərdə pik həddə çatır

Metodlar:

 Invoice Value hesablaması:
  `Invoice Value = ((Quantity * Avg_Price) * (1 - Discount_pct)) * (1 + GST) + Delivery_Charges`
 Average Order Value, Profit Margin və Purchase Frequency ölçüldü.

2️⃣ Müştəri Segmentasiyası (RFM və LTV)

RFM Segmentasiyası ilə müştərilər Premium, Gold, Silver və Standard qruplarına ayrıldı.

Recency: Son alış tarixi
Frequency: Alış sayı
Monetary: Xərclənən məbləğ
LTV Analizi   Müştərilərin uzunmüddətli gəlir potensialı müəyyən edildi.

   Yüksək LTV → uzunmüddətli prioritet müştəri
   Orta və aşağı LTV → uyğun strategiyalar üçün hədəfləndi

 3️⃣ Next Purchase Day Analizi

 Müştərinin növbəti alışını proqnozlaşdırmaq üçün ortalama alış intervalı hesablandı.
 Müştərilər qruplaşdırıldı:

   0–30 gün, 30–60 gün, 60+ gün
 Bu, marketing kampaniyalarının vaxtını optimallaşdırmağa imkan verir.

4️⃣ Cohort Analizi

 Müştərilər ilk alış etdikləri aya görə qruplaşdırıldı.
 Retention və alış tendensiyaları izlənildi.
 Hər ayın cohortu üzrə müştəri davranış nümunələri və retention strategiyaları müəyyən edildi.

 5️⃣ Market Basket / Cross-Selling Analizi

 Hangi məhsulların birgə satın alındığı müəyyən edildi.
Ən çox birlikdə alınan məhsullar marketinq və bundle kampaniyaları üçün prioritetləndirildi.

 6️⃣ Marketinq və Gəlir Təsiri

 Aylıq marketing spend və gəlir müqayisəsi aparıldı.
 Marketing spend-in gəlirə təsiri faizlə göstərildi.
 Online vs Offline xərclərin effektivliyi analiz edildi.

 

🔹 Əsas KPI-lar və Hesablamalar

Revenue: Hər tranzaksiya üzrə gəlir
Average Order Value: Müştəri başına orta sifariş məbləği
Profit Margin: Satışın qazanc faizi
Purchase Frequency: Müştərinin orta alış sayı
Repeat Rate: Təkrar alış edən müştərilərin faizi
Churn Rate: Müştərilərin illik abonent dayandırma faizi
Customer Lifetime Value (LTV): Müştərinin uzunmüddətli monetar dəyəri

🔹 Business Impact

Müştəri segmentasiyası marketinq strategiyasını optimallaşdırdı.
Endirim və kampaniyaların gəlir üzərində təsiri izlənildi.
Cohort və Next Purchase Day analizi ilə müştəri retention artırıldı.
 Market Basket analizi ilə cross-selling və bundling imkanları müəyyən edildi.


