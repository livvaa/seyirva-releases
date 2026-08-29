<p align="center">
  <img src="screenshots/kanal-listesi.png" width="720" alt="Seyirva — kanal listesi ve canlı yayın" />
</p>

<h1 align="center">Seyirva</h1>

<p align="center">
  Google TV · Android TV · Tablet · Telefon için ücretsiz canlı yayın uygulaması
</p>

<p align="center">
  <a href="https://github.com/livvaa/seyirva-releases/releases/latest">
    <img src="https://img.shields.io/github/v/release/livvaa/seyirva-releases?style=for-the-badge&label=İndir&color=1DB954" alt="Son sürüm" />
  </a>
</p>

---

## Nedir?

**Seyirva**, Google TV, Android TV kutuları, tablet ve telefonlarda çalışan bir canlı TV ve kamera yayın uygulamasıdır. Hiçbir video veya yayın barındırmaz; yalnızca [iptv-org](https://github.com/iptv-org/iptv) tarafından toplanan kamuya açık yayın bağlantılarını oynatır.

Tek bir APK tüm cihazlarda çalışır — televizyonda kumandayla, tablet ve telefonda dokunmatik kontrollerle.

## Öne Çıkan Özellikler

| Özellik | Açıklama |
|---|---|
| 📺 **200+ ülke** | Dünyanın dört bir yanından canlı TV kanalları |
| 📷 **Canlı kameralar** | 20 ülkeden trafik, sahil ve şehir kameraları |
| 📋 **Program rehberi (EPG)** | XMLTV tabanlı, şimdi ve sonraki program bilgisi |
| 🔍 **Kanal ve ülke arama** | TV kumandasıyla bile kullanılabilen sanal klavye |
| 🔄 **Otomatik sunucu geçişi** | Yayın kesilirse alternatif sunucuya otomatik geçiş |
| 🩺 **Sağlık taraması** | Çalışmayan kanallar arka planda tespit edilip listeden çıkar |
| 🏠 **Google TV entegrasyonu** | Ana ekranda "Şimdi Yayında" ve "İzlemeye devam et" kartları |
| 🌈 **Çevresel ışıklandırma** | Telefonda yayının rengi ekranın boş alanlarına yayılır |
| 🔄 **Otomatik güncelleme** | Yeni sürüm arka planda indirilir, açılışta kurulur |

## Ekran Görüntüleri

<p align="center">
  <img src="screenshots/kanal-listesi.png" width="400" alt="Kanal listesi" />
  <img src="screenshots/ulke-secimi.png" width="400" alt="Ülke seçimi" />
</p>
<p align="center">
  <img src="screenshots/bilgi-cubugu.png" width="400" alt="Bilgi çubuğu ve EPG" />
</p>

## Kurulum

### 1. APK'yı İndir

[**Releases**](https://github.com/livvaa/seyirva-releases/releases/latest) sayfasından en son `Seyirva-X.Y.Z.apk` dosyasını indirin.

### 2. Cihaza Yükle

#### Google TV / Android TV Kutusu
1. APK'yı bir USB belleğe kopyalayın veya **Send Files to TV** gibi bir uygulamayla cihaza gönderin.
2. Bir dosya yöneticisi ile APK'yı açın.
3. İlk seferde "Bilinmeyen uygulamalara izin ver" istenir — izni açın.
4. Kurulumu tamamlayın.

#### Tablet / Telefon
1. APK'yı doğrudan tarayıcıdan indirin.
2. Bildirim çubuğundan veya dosya yöneticisinden açın.
3. Gerekirse "Bilinmeyen kaynaklara izin ver" seçeneğini açın.
4. Kurulumu tamamlayın.

### 3. Kullanmaya Başla

İlk açılışta ülke seçimi yapın — uygulama o ülkedeki mevcut kanalları yükleyecek ve yayın başlayacak.

## Kumanda Kullanımı (TV)

| Tuş | İşlev |
|---|---|
| ◀ Sol | Kanal listesini aç |
| ▶ Sağ | Ayarları aç |
| ▲▼ Yukarı/Aşağı | Kanal değiştir |
| OK | Bilgi çubuğu / seç |
| Geri | Menüyü kapat / çık |
| 🔴 Kırmızı | Altyazı aç/kapat |
| 🟢 Yeşil | Ses kanalı değiştir |
| 🟡 Sarı | Program rehberi |
| 🔵 Mavi | Canlı yayına dön |

## Dokunmatik Kullanım (Tablet / Telefon)

| Hareket | İşlev |
|---|---|
| Sağa kaydır | Kanal listesini aç |
| Sola kaydır | Ayarları aç |
| Yukarı/Aşağı kaydır | Kanal değiştir |
| Dokun | Bilgi çubuğu |

## Güncelleme

Seyirva kendi kendini günceller:

1. Açılışta yeni sürüm olup olmadığını kontrol eder.
2. Varsa APK'yı arka planda sessizce indirir.
3. Sonraki açılışta kurulum ekranı gösterir.

Güncelleme zorunludur — yan yüklenen bir uygulamada atlanabilen güncelleme pratikte hiç kurulmuyor.

## Sorun Giderme

| Sorun | Çözüm |
|---|---|
| "Paket çakışması" hatası | Uygulamayı kaldırıp yeniden kurun (imza değişikliği) |
| Kanal açılmıyor | Başka bir kanala geçip tekrar deneyin; yayın kaynağı geçici olarak çökebilir |
| Güncelleme kurulamıyor | Ayarlar → Uygulamalar → Seyirva → "Bilinmeyen uygulamalara izin ver" |

## Yasal Uyarı

Seyirva hiçbir video veya yayın barındırmaz. Tüm yayınlar ve içerik hakları ilgili hak sahiplerine aittir. Uygulama yalnızca kamuya açık kaynaklardan toplanan bağlantıları oynatır.

---

<details>
<summary><strong>Geliştirici Notları</strong></summary>

### update.json

Bu depodaki `update.json`, uygulamanın açılışta okuduğu güncelleme bildirimidir:

| Alan | Anlamı |
|---|---|
| `versionCode` | Yüklü sürümden büyükse güncelleme indirilir |
| `versionName` | Kurulum ekranında gösterilir |
| `apkUrl` | APK'nın doğrudan HTTPS adresi |
| `sizeBytes` | İndirilen dosya bu boyutta değilse kurulum reddedilir |
| `notes` | Kurulum ekranında gösterilen değişiklik notu |
| `mandatory` | `true` ise açılışta kurulum ekranı zorunlu gelir |

### Yeni sürüm yayınlama

1. Kaynak depoda sürümü yükselt, `assembleRelease` ile imzalı APK üret.
2. Bu depoda `vX.Y.Z` etiketiyle bir release aç, APK'yı `Seyirva-X.Y.Z.apk` adıyla ekle.
3. `update.json`'u yeni `versionCode`, `versionName`, `apkUrl` ve `sizeBytes` ile güncelle.

APK'lar her zaman aynı anahtarla imzalanmalıdır; imza değişirse cihazlar güncellemeyi reddeder ve kullanıcının elle kaldırıp kurması gerekir.

</details>
