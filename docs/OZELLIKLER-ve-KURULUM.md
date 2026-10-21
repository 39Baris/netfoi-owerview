# Netfoi — Sistem Özellikleri & Teknik Kılavuz

Bu belge, **Netfoi Film, Dizi & Canlı TV Streaming Scripti** altyapısının teknik özelliklerini, modüllerini ve sistem gereksinimlerini özetler.

---

## 🛠️ Sistem Gereksinimleri

Script modern JavaScript ve Node.js ekosistemi üzerinde çalışır. Standart bir VPS / VDS sunucuya veya bulut platformlarına (Vercel, Railway, Coolify, Docker vb.) dakikalar içinde kurulabilir.

- **Node.js**: v20.x veya v22.x LTS
- **Veritabanı**: SQLite (yerel tek dosya / hafif kullanım) veya PostgreSQL / MySQL (yüksek trafikli prodüksiyon)
- **Sunucu**: Linux (Ubuntu 22.04+ / Debian) veya Windows Server, en az 1 GB RAM (2 GB+ önerilir)
- **Paket Yöneticisi**: npm, pnpm veya yarn

---

## 📦 Modül ve Özellik Detayları

### 1. Canlı TV & IPTV Proxy Motoru
- **CORS-Free Proxy Route (`/api/live-tv/stream`)**:
  - Xtream Codes URL formatlarını (`host/user/pass/id`, `host/user/pass/id.m3u8`, `host/live/user/pass/id.m3u8`) otomatik tespit eder ve normalize eder.
  - Upstream 302 yönlendirmelerini takip eder.
  - Playlist içerisindeki `.ts` video segmentlerini proxy üzerinden yeniden yazarak tarayıcıda karma içerik (mixed content) ve CORS hatalarını ortadan kaldırır.
- **Toplu Kanal Yönetimi**:
  - `KATEGORI\tISIM\tURL` formatında binlerce satırlık IPTV verisini anında parse eder.
  - Sayfalamalı, aranabilir ve kategori filtreli önizleme tablosu sunar.
  - Tek tıkla veritabanına toplu kayıt oluşturur.
- **Özel HLS Live Player**:
  - HLS.js entegrasyonu ile otomatik oynatma (autoplay).
  - Tarayıcı ses politikasını algılayıp sessiz başlatma ve tek tıkla ses açma bildirimi ("Sesi Aç").
  - Canlı yayın senkronizasyon butonu.
  - Çoklu ses parçası ve yayın kalitesi seçici menüsü.

### 2. Film & Dizi Yönetimi
- TMDB (The Movie Database) API entegrasyonu ile otomatik meta veri, afiş ve arka plan çekme.
- Dizi sezon ve bölüm yönetimi (özel küçük resim, başlık ve bölüm sıralaması).
- Kategori ve tür (genre) ilişkilendirme.
- Öne çıkan içerik (`isFeatured`) belirleme.
- Ziyaretçi izleme geçmişi ve favoriler listesi.

### 3. Görünüm & Tema Motoru
- **Midnight**: Klasik, simsiyah zemin üzerinde elektrik mavisi vurgular.
- **Obsidian**: Koyu gri/yeşil paneller ve turkuaz detaylar.
- **Apex Gold (IMAX)**: Derin karbon siyahı zemin, kehribar-altın renk paleti, 88vh dev sinema sahnesi ve canlı TV hızlı vitrini.
- Admin panelden yapılan tema değişikliği `data-theme` özniteliği ile anında tüm ziyaretçilere yansır.

### 4. Güvenlik ve Yönetim
- **Erişim Kodu (Gatekeeper)**: Siteyi kapalı devre tutmak isteyenler için şifre koruma katmanı.
- **Bakım Modu**: Tek tıkla bakım sayfası yayını; adminler çalışmaya devam edebilir.
- **Yorum Onay Mekanizması**: İstenmeyen yorumları önlemek için admin denetim kuyruğu.
- **Admin Eylem Günlüğü (Audit Log)**: Yapılan tüm değişikliklerin kaydedildiği detaylı log sistemi.

---

## 🚀 Kurulum Adımları (Lisans Alıcıları İçin Özet)

1. Depoyu sunucunuza çekin:
   ```bash
   git clone <size-verilen-ozel-repo-adresi> netfoi
   cd netfoi
   ```
2. Bağımlılıkları yükleyin:
   ```bash
   npm install
   ```
3. `.env` yapılandırma dosyasını doldurun:
   ```env
   DATABASE_URL="postgresql://user:password@localhost:5432/netfoi"
   NEXTAUTH_SECRET="guclu-bir-secret-anahtari"
   TMDB_API_KEY="tmdb-api-anahtariniz"
   ```
4. Veritabanını hazırlayın ve derleyin:
   ```bash
   npm run db:push
   npm run build
   ```
5. PM2 veya Docker ile yayına alın:
   ```bash
   pm2 start npm --name "netfoi" -- start
   ```

---

## 📞 Satın Alma & Destek
- **Geliştirici:** [@39Baris](https://github.com/39Baris)
- Satın alım sonrası kurulum, özel alan adı yönlendirme ve teknik yapılandırma desteği sağlanmaktadır.
