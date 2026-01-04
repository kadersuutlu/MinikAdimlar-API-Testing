# Minik Adımlar - API Test Automation Project 🛠️

Bu repository, **Juniors** topluluğu bünyesinde geliştirilen **Minik Adımlar** (Bebek Gelişim Takip Uygulaması) projesinin backend servisleri için hazırladığım kapsamlı test süreçlerini içermektedir. Proje, manuel testlerden otomasyona geçiş sürecini ve profesyonel bir API test mimarisinin nasıl kurgulandığını sergilemek amacıyla hazırlanmıştır.

---

## 📌 Proje Kapsamı ve İlerleme Durumu
Test süreçleri, uygulamanın iş mantığına (business logic) uygun olarak 6 stratejik faza ayrılmıştır. Her fazın tamamlanmasıyla birlikte ilgili koleksiyonlar repoya eklenecektir:

- [x] **Faz 1: Auth & User Management** (Tamamlandı ✅)
    - *Kullanıcı kayıt, giriş, şifre yenileme ve profil yönetimi süreçleri.*
- [ ] **Faz 2: Core Data Management (Baby & Growth)** (Yükleniyor... ⏳)
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

## 🔐 Faz 1 Detayları: Auth & User Management
Bu aşamada kullanıcının güvenli bir şekilde sisteme dahil olması ve yetkilendirme süreçlerinin hatasız çalışması test edilmiştir.

### Test Edilen Uç Noktalar (Endpoints):
* `POST /auth/register` - Yeni kullanıcı kaydı ve veri validasyonları.
* `POST /auth/login` - Giriş işlemleri ve Access Token yönetimi.
* `POST /auth/refresh-token` - Oturum yenileme senaryoları.
* `POST /auth/forgot-password` & `POST /auth/reset-password` - Şifre kurtarma akışları.

### Uygulanan Teknik Yetkinlikler:
* **Dynamic Environment Variables:** Login sonrası alınan `access_token`, Postman scriptleri ile otomatik olarak ortama atanmış ve sonraki tüm isteklere dinamik olarak aktarılmıştır.
* **Pre-request Scripts:** Test verisi çeşitliliği sağlamak amacıyla JavaScript ile dinamik veri üretimi gerçekleştirilmiştir.
* **Tests & Assertions:**
    * **Status Code Validation:** Yanıt kodlarının kontratlara uygunluğu.
    * **JSON Schema Validation:** Response gövdesinin yapısal doğruluğu.
    * **Response Time Assertions:** Performans kriterlerinin denetlenmesi.

---

## 🛠 Kullanılan Araçlar
* **Postman** (API Testing & Documentation)
* **JavaScript** (Postman Scripting)
* **Markdown** (Project Documentation)

---

## 🚀 Nasıl Çalıştırılır?
1. Repository içerisindeki `.json` formatındaki koleksiyon dosyasını bilgisayarınıza indirin.
2. Postman uygulamasını açın ve **Import** butonuna basarak dosyayı seçin.
3. Testleri çalıştırmak için bir `environment` oluşturup `base_url` tanımlamanız önerilir.

---
> **Not:** Bu çalışma sadece test otomasyon kurgusunu ve QA yetkinliklerini sergilemek amacıyla paylaşılmıştır. Projenin kaynak kodlarını veya hassas kullanıcı verilerini içermez.
