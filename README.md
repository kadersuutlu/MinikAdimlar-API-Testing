# Minik Adımlar - API Test Automation Project 🛠️

Bu repository, **Juniors** topluluğu bünyesinde geliştirilen **Minik Adımlar** (Bebek Gelişim Takip Uygulaması) projesinin backend servisleri için hazırladığım kapsamlı test süreçlerini içermektedir. Proje, manuel testlerden otomasyona geçiş sürecini ve profesyonel bir API test mimarisinin nasıl kurgulandığını sergilemek amacıyla hazırlanmıştır.

---

## 📌 Proje Kapsamı ve İlerleme Durumu
Test süreçleri, uygulamanın iş mantığına (business logic) uygun olarak 6 stratejik faza ayrılmıştır:

- [x] **Faz 1: Auth & User Management** (Tamamlandı ✅)
    - *Kullanıcı kayıt, giriş, şifre yenileme ve profil yönetimi süreçleri.*
- [x] **Faz 2: Core Data Management (Baby & Growth)** (Tamamlandı ✅)
    - *Bebek profili oluşturma ve fiziksel gelişim (Boy, Kilo, Baş çevresi) takibi.*
- [ ] **Faz 3: Daily Activity Tracking** (Planlanıyor 📅)
    - *Beslenme (Emzirme/Biberon), Uyku ve Bez değişimi süreçleri.*
- [ ] **Faz 4: Health & Medical Logging** (Planlanıyor 📅)
    - *Sağlık kayıtları, kategori bazlı takip ve tıbbi geçmiş.*
- [ ] **Faz 5: Content & Educational Services** (Planlanıyor 📅)
    - *İçerik listeleme, arama, okuma listeleri ve filtreleme servisleri.*
- [ ] **Faz 6: Smart Services & Reporting** (Planlanıyor 📅)
    - *Etkinlik takvimi, hatırlatıcılar, Recap (Özet) raporları ve bildirim servisleri.*

---

## 🔐 Öne Çıkan Teknik Detaylar (Faz 1 & 2)
Bu aşamalarda API'ların hem güvenliği hem de veri işleme yetenekleri test edilmiştir.

### Uygulanan Teknik Yetkinlikler:
* **Dynamic Environment Variables:** Login sonrası alınan `access_token`, Postman scriptleri ile otomatik olarak ortama atanmış ve tüm isteklere dinamik olarak aktarılmıştır.
* **Complex Data Handling:** Faz 2 kapsamında bebek profili oluşturma ve bu profile bağlı boy/kilo verilerinin ilişkilendirilmesi test edilmiştir.
* **Pre-request Scripts:** Test verisi çeşitliliği için JavaScript ile dinamik veri (faker benzeri) üretimi yapılmıştır.
* **Advanced Assertions:** * **JSON Schema Validation:** API yanıtlarının yapısal doğruluğu.
    * **Performance Testing:** Yanıt sürelerinin belirlenen limitler (ms) altında kalması.

---

## 📱 Roadmap: Phase 2 - Mobile Automation Integration (New! 🚀)

API testlerine paralel olarak projenin mobil ayağı için otomasyon süreci başlatılmıştır. 

* **Altyapı:** Expo projesi native yapıya (`Prebuild`) geçirilerek Android ortamı hazırlandı.
* **Appium & Inspector:** `UiAutomator2` driver ile emülatör bağlantısı sağlandı, Appium Inspector üzerinden element tespiti ve E2E (uçtan uca) senaryo kurgulama aşamasına geçildi.

---

## 🛠 Kullanılan Araçlar
* **Postman & JavaScript** (API Automation)
* **Appium & UiAutomator2** (Mobile Automation)
* **Android Studio & Emulator** (Test Environment)

---
> **Not:** Bu çalışma sadece test otomasyon kurgusunu ve QA yetkinliklerini sergilemek amacıyla paylaşılmıştır. Projenin kaynak kodlarını veya hassas kullanıcı verilerini içermez.
