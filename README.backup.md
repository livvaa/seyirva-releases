# Seyirva — dağıtım

Seyirva'nın güncelleme bildirimi ve APK dosyaları. Kaynak kod ayrı, gizli bir depodadır.

`update.json` uygulamanın açılışta okuduğu bildirimdir:

| Alan | Anlamı |
|---|---|
| `versionCode` | Yüklü sürümden büyükse güncelleme indirilir |
| `versionName` | Kurulum ekranında gösterilir |
| `apkUrl` | APK'nın doğrudan HTTPS adresi |
| `sizeBytes` | İndirilen dosya bu boyutta değilse kurulum reddedilir |
| `notes` | Kurulum ekranında gösterilen değişiklik notu |
| `mandatory` | `true` ise açılışta kurulum ekranı zorunlu gelir |

## Yeni sürüm yayınlama

1. Kaynak depoda sürümü yükselt, `assembleRelease` ile imzalı APK üret.
2. Bu depoda `vX.Y.Z` etiketiyle bir release aç, APK'yı `Seyirva-X.Y.Z.apk` adıyla ekle.
3. `update.json`'u yeni `versionCode`, `versionName`, `apkUrl` ve `sizeBytes` ile güncelle.

APK'lar her zaman aynı anahtarla imzalanmalıdır; imza değişirse cihazlar güncellemeyi
reddeder ve kullanıcının elle kaldırıp kurması gerekir.
