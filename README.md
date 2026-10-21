<p align="center"><sub>🌐 <b>Türkçe</b> · <a href="README.en.md">English</a></sub></p>

<p align="center">
  <img src="screenshots/01-anasayfa.png" alt="Netfoi — Film, Dizi & Canlı TV Streaming Scripti" width="100%">
</p>

<div align="center">

# Netfoi — Film, Dizi & Canlı TV (IPTV) Platform Scripti

**Yeni nesil sinematik VOD & Canlı TV yayın altyapısı.** Film, dizi, belgesel arşivi ve dahili **CORS-Free Xtream Codes IPTV proxy motoru** ile anahtar teslim streaming scripti.

Next.js 16 · React 19 · TypeScript · Tailwind CSS · Prisma ORM · HLS.js

<br>

<a href="https://t.me/jzlvv"><img src="https://img.shields.io/badge/Telegram-@jzlvv-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram"></a>
&nbsp;
<a href="https://github.com/39Baris"><img src="https://img.shields.io/badge/GitHub-@39Baris-111827?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"></a>
&nbsp;
<a href="docs/OZELLIKLER-ve-KURULUM.md"><img src="https://img.shields.io/badge/Özellikler%20%26%20Detaylar-1f6feb?style=for-the-badge&logo=readme&logoColor=white" alt="Özellikler & Detaylar"></a>

<br><br>

<img src="https://img.shields.io/badge/Canl%C4%B1%20TV%20%26%20IPTV-E50914?style=for-the-badge" alt="Canlı TV & IPTV">
<img src="https://img.shields.io/badge/Xtream%20Codes%20Proxy-F59E0B?style=for-the-badge" alt="Xtream Proxy">
<img src="https://img.shields.io/badge/3x%20Tema%20Se%C3%A7ene%C4%9Fi-8B5CF6?style=for-the-badge" alt="3x Tema Seçeneği">
<img src="https://img.shields.io/badge/TMDB%20API%20Botu-0EA5E9?style=for-the-badge" alt="TMDB Botu">
<img src="https://img.shields.io/badge/PWA%20Destekli-10B981?style=for-the-badge" alt="PWA Destekli">

<br>

<img alt="Next.js 16" src="https://img.shields.io/badge/Next.js%2016-000000?style=flat&logo=nextdotjs&logoColor=white">
<img alt="React 19" src="https://img.shields.io/badge/React%2019-20232A?style=flat&logo=react&logoColor=61DAFB">
<img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-007ACC?style=flat&logo=typescript&logoColor=white">
<img alt="Tailwind CSS" src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white">
<img alt="Prisma" src="https://img.shields.io/badge/Prisma_ORM-2D3748?style=flat&logo=prisma&logoColor=white">
<img alt="HLS.js" src="https://img.shields.io/badge/HLS.js-FF0055?style=flat&logoColor=white">

</div>

> [!IMPORTANT]
> **📢 Satın alma & lisanslama:** Telegram: [@jzlvv](https://t.me/jzlvv) üzerinden veya GitHub profilindeki bağlantılardan doğrudan iletişime geçebilirsiniz.
>
> **📖 Ayrıntılı özellikler & gereksinimler:** [docs/OZELLIKLER-ve-KURULUM.md](docs/OZELLIKLER-ve-KURULUM.md)
>
> 🔒 **Tanıtım Vitrini:** Kaynak kodlar ve ticari modüller özel mülkiyettir. Bu depo yalnızca ekran görüntülerini ve öne çıkan sistem yeteneklerini sergilemektedir.

---

## 📸 Ekran Görüntüleri

| 🎬 88vh IMAX Sinema Ana Sayfası | 📺 Canlı TV & IPTV Oynatıcı |
|---|---|
| ![Ana Sayfa](screenshots/01-anasayfa.png) | ![Canlı TV](screenshots/02-canli-tv.png) |

| 🍿 Film & Dizi Kataloğu | ⚙️ Yönetim Paneli Dashboard |
|---|---|
| ![Filmler](screenshots/03-filmler-katalogu.png) | ![Admin Panel](screenshots/04-admin-panel.png) |

| 📡 Canlı TV & Kanal Yönetimi | ⚡ Toplu Kanal Ekleme Sihirbazı |
|---|---|
| ![Canlı TV Yönetimi](screenshots/05-admin-canli-tv.png) | ![Toplu Kanal Ekleme](screenshots/06-admin-toplu-ekleme.png) |

<p align="center">
  <img src="screenshots/07-admin-ayarlar.png" width="900" alt="Yönetim Paneli Tema Seçici ve Sistem Ayarları">
  <br>
  <em>Görünüm Ayarları: Tek tıkla Midnight (Mavi), Obsidian (Yeşil) ve Apex Gold (IMAX Altın) temaları arasında anlık geçiş</em>
</p>

### 📱 Mobil Görünüm (Ultra Responsive PWA)

<p align="center">
  <img src="screenshots/08-mobil-anasayfa.png" width="280" alt="Mobil Ana Sayfa">
  &nbsp;&nbsp;
  <img src="screenshots/09-mobil-canli-tv.png" width="280" alt="Mobil Canlı TV">
  &nbsp;&nbsp;
  <img src="screenshots/10-mobil-filmler.png" width="280" alt="Mobil Film Kataloğu">
</p>

---

## ⭐ Öne Çıkan Özellikler

### 📺 Özel Canlı TV & IPTV Proxy Motoru
- **CORS & Token Bypass**: Xtream Codes protokolündeki 302 token yönlendirmelerini, Cloudflare engellerini ve CORS kısıtlamalarını sunucu taraflı aşan özel proxy mimarisi.
- **Otomatik HLS / m3u8 Rewrite**: `.m3u8` playlist segmentlerini dinamik proxy URL'lerine dönüştürerek tarayıcıda %100 kesintisiz oynatma.
- **Toplu Kanal Yükleme Sihirbazı**: `KATEGORI\tISIM\tURL` formatında binlerce kanalı (5.000+ test edildi) tek seferde saniyeler içinde anlık canlı tablo önizlemesiyle sisteme aktarma.
- **Özel HLS Live Player**: Düşük gecikmeli canlı yayın modu, otomatik sessiz başlatma kurtarması, ses kanalı & kalite değiştirme, tam ekran desteği.
- **Aç/Kapa Master Switch**: Admin panelden Canlı TV modülünü tek tıkla site genelinde ve menüde aktif/pasif edebilme.

### 🎬 Film & Dizi Streaming Mimarisi
- **Çoklu Video Kaynağı**: Doğrudan video URL (HLS / MP4), iframe / embed desteği ve harici kaynaklar.
- **Gelişmiş Video Oynatıcı**: Çoklu dil, altyazı desteği, hız kontrolü, kaldığın yerden devam etme.
- **TMDB API Otomatik İçerik Botu**: Tek tıkla afiş, arka plan, özet, oyuncu kadrosu, tür ve puan verilerini otomatik içe aktarma.
- **Sezon & Bölüm Yönetimi**: Diziler için pratik sezon ve bölüm ekleme, sıralama, özel küçük resimler.

### 🎨 3x Dahili Görünüm Teması (Admin Panelden Anlık Geçiş)
- 🌌 **Midnight**: Klasik sinematik siyah zemin ve elektrik mavisi vurgular.
- 🌿 **Obsidian**: Koyu arduvaz ve canlı neon turkuaz detaylar.
- 👑 **Apex Gold (IMAX)**: Karbon siyahı, sıcak kehribar-altın vitrin ve tam ekran sinema sahnesi.

### 🛡️ Güvenlik, Üyelik & Yönetim
- **Erişim Kodu Modu**: Siteyi özel kılmak için şifre / erişim kodu zorunluluğu açıp kapatabilme.
- **Bakım Modu**: Ziyaretçilere özel bakım sayfası gösterirken adminlere kesintisiz erişim.
- **Yorum & Denetim Sistemi**: Spoiler uyarısı, beğeni sistemi ve admin onay mekanizması.
- **İzleme Listesi & Favoriler**: Kullanıcıların kendi özel listelerini oluşturabilmesi.
- **PWA (Progressive Web App)**: Mobilde uygulama gibi ana ekrana eklenebilme, çevrimdışı önbellekleme desteği.

---

## 🧩 Teknoloji Mimarisi

| Katman | Teknoloji | Açıklama |
|---|---|---|
| **Frontend** | Next.js 16 (App Router), React 19 | Server Components, Streaming SSR, Sıfır Gecikme |
| **Styling** | Tailwind CSS 3.4 | Tam responsive, GPU hızlandırmalı modern UI |
| **Backend & API** | Next.js Route Handlers | Node.js tabanlı yüksek hızlı proxy ve REST API |
| **Veritabanı** | Prisma ORM (SQLite / PostgreSQL) | Esnek, taşınabilir ve yüksek performanslı veri modeli |
| **Medya Motoru** | HLS.js & Özel LiveTvPlayer | Düşük gecikmeli IPTV ve VOD streaming |
| **Kimlik Doğrulama** | NextAuth.js v5 | Rol tabanlı oturum yönetimi (Admin / Üye) |

---

## 🔎 Kullanım Alanları

Netfoi, aşağıdaki projeler için anahtar teslim, yüksek performanslı hazır bir altyapıdır:
- **Premium Film & Dizi İzleme Portalı** (VOD platformu)
- **Web Tabanlı IPTV & Canlı Yayın Servisi** (Xtream Codes & M3U yayınları)
- **Topluluk / Kapalı Devre Sinema Kulübü** (Erişim kodu korumalı)
- **Kişisel Medya Sunucusu Arayüzü**

---

## 💼 Satın Alma & İletişim

Netfoi lisansı ve kaynak kod paketi satıştadır. Detaylı bilgi, canlı demo ve fiyatlandırma için iletişime geçebilirsiniz:

- ✈️ **Telegram:** [@jzlvv](https://t.me/jzlvv) *(Hızlı Yanıt)*
- 💬 **GitHub:** [@39Baris](https://github.com/39Baris)

---

<sub><b>Anahtar kelimeler:</b> film scripti, dizi scripti, iptv scripti, canli tv scripti, nextjs streaming script, film izleme sitesi yazilimi, xtream codes web player, hls m3u8 proxy player, vod scripti, film dizi botu, netflix klonu script.</sub>

## 📄 Lisans
Ticari / Özel Yazılım — **Tüm Hakları Saklıdır**. Kaynak kodlar izin alınmaksızın çoğaltılamaz veya dağıtılamaz.
