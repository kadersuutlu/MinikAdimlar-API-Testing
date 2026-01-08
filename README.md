# Minik Adımlar - API Test Automation Project 🛠️

Bu repository, **Juniors** topluluğu bünyesinde geliştirilen **Minik Adımlar** (Bebek Gelişim Takip Uygulaması) projesinin backend servisleri için hazırladığım kapsamlı test süreçlerini içermektedir. Proje, manuel testlerden otomasyona geçiş sürecini ve profesyonel bir API test mimarisinin nasıl kurgulandığını sergilemek amacıyla hazırlanmıştır.

---

## 📌 Proje Kapsamı ve İlerleme Durumu
Test süreçleri, uygulamanın iş mantığına (business logic) uygun olarak 6 stratejik faza ayrılmıştır:

- [x] **Faz 1: Auth & User Management** (Tamamlandı ✅)
- [x] **Faz 2: Core Data Management (Baby & Growth)** (Tamamlandı ✅)
- [x] **Faz 3: Daily Activity Tracking (Nutrition, Sleep, Diaper)** (Tamamlandı ✅)
- [x] **Faz 4: Health & Medical Logging** (Tamamlandı ✅)
- [ ] **Faz 5: Content & Educational Services** (Planlanıyor 📅)
- [ ] **Faz 6: Smart Services & Reporting** (Planlanıyor 📅)

---

## 🔐 Öne Çıkan Teknik Detaylar (Faz 1 - 4)
Bu aşamalarda API'ların güvenliği, iş mantığı (business logic) ve veri tutarlılığı uçtan uca test edilmiştir.

### Uygulanan Teknik Yetkinlikler:
* **Dynamic Token Management:** Login sonrası alınan `accessToken` ve `refreshToken` değerleri, Postman scriptleri ile otomatik olarak ortama atanmış; oturum yenileme (Refresh Token) akışları dinamik değişkenlerle otomatize edilmiştir.
* **End-to-End Activity Tracking:** Faz 3 & 4 kapsamında beslenme, uyku, bez değişimi ve sağlık kayıtlarının birbiriyle ilişkili çalışma mantığı (CRUD operasyonları) test edilmiştir.
* **Bug Detection & Documentation:** Yapılan testler sonucunda; boş veri setlerinde 400 hatası dönmesi, yetki kontrollerindeki (401 vs 403) tutarsızlıklar ve hatalı iş mantığı (aktif kayıt varken yeni kayıt başlatılabilmesi) gibi kritik bulgular tespit edilmiş ve detaylıca raporlanmıştır.
* **Advanced Data Validation:** * **JSON Schema Validation:** API yanıtlarının veri tipleri ve yapısal doğruluğu denetlenmiştir.
    * **Boundary Value Analysis:** Negatif test senaryoları ile (geçersiz tarih, hatalı enum, negatif değerler) sistemin dayanıklılığı ölçülmüştür.
* **Pre-request & Post-res Scripts:** JavaScript kullanılarak dinamik test verisi üretilmiş ve her istek sonrası otomatik statü kodu kontrolleri yapılmıştır.
---

## 🛠 Kullanılan Araçlar
* **Postman** (API Automation)
* **JavaScript** (Scripting & Assertions)
* **Markdown** (Documentation)

---
> **Not:** Bu çalışma sadece test otomasyon kurgusunu ve QA yetkinliklerini sergilemek amacıyla paylaşılmıştır. Projenin kaynak kodlarını veya hassas kullanıcı verilerini içermez.
