# Minik Adımlar - API Test Automation Project 🛠️

Bu repository, **Juniors** topluluğu bünyesinde geliştirilen **Minik Adımlar** (Bebek Gelişim Takip Uygulaması) projesinin backend servisleri için hazırladığım kapsamlı test süreçlerini içermektedir. Proje, manuel testlerden otomasyona geçiş sürecini ve profesyonel bir API test mimarisinin nasıl kurgulandığını sergilemek amacıyla hazırlanmıştır.

---

## 📌 Proje Kapsamı ve İlerleme Durumu
Test süreçleri, uygulamanın iş mantığına (business logic) uygun olarak 6 stratejik faza ayrılmıştır:

- [x] **Faz 1: Auth & User Management** (Tamamlandı ✅)
    - *Kullanıcı kayıt, giriş, şifre yenileme ve profil yönetimi süreçleri.*
- [x] **Faz 2: Core Data Management (Baby & Growth)** (Tamamlandı ✅)
    - *Bebek profili oluşturma ve fiziksel gelişim (Boy, Kilo, Baş çevresi) takibi.*
- [ ] **Faz 3: Daily Activity Tracking (Nutrition, Sleep, Diaper)** (Planlanıyor 📅)
- [ ] **Faz 4: Health & Medical Logging** (Planlanıyor 📅)
- [ ] **Faz 5: Content & Educational Services** (Planlanıyor 📅)
- [ ] **Faz 6: Smart Services & Reporting** (Planlanıyor 📅)

---

## 🔐 Öne Çıkan Teknik Detaylar (Faz 1 & 2)
Bu aşamalarda API'ların hem güvenliği hem de veri işleme yetenekleri test edilmiştir.

### Uygulanan Teknik Yetkinlikler:
* **Dynamic Environment Variables:** Login sonrası alınan `accessToken` ve `refreshToken`, Postman scriptleri (`pm.environment.set`) ile otomatik olarak ortama atanmış ve tüm yetkilendirme gerektiren isteklere dinamik olarak aktarılmıştır.
* **Complex Data Handling:** Faz 2 kapsamında bebek profili oluşturma ve bu profile bağlı boy/kilo verilerinin ilişkilendirilmesi test edilmiştir.
* **Pre-request Scripts:** Test verisi çeşitliliği sağlamak amacıyla JavaScript ile dinamik veri (random mail, name vb.) üretimi yapılmıştır.
* **Advanced Assertions:** * **JSON Schema Validation:** API yanıtlarının yapısal ve tip bazlı doğruluğu.
    * **Status Code & Performance:** Yanıt kodlarının kontratlara uygunluğu ve yanıt sürelerinin (ms) denetlenmesi.

---

## 🛠 Kullanılan Araçlar
* **Postman** (API Automation)
* **JavaScript** (Scripting & Assertions)
* **Markdown** (Documentation)

---
> **Not:** Bu çalışma sadece test otomasyon kurgusunu ve QA yetkinliklerini sergilemek amacıyla paylaşılmıştır. Projenin kaynak kodlarını veya hassas kullanıcı verilerini içermez.
