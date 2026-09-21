# LAGORA — GitHub Pages paket

Bu paket tek dosyalı LAGORA uygulamasını HTTPS üzerinden yayınlamak için hazırlanmıştır.

## İçerik
- `index.html` — mevcut LAGORA uygulaması
- `manifest.webmanifest` — iPhone/Android ana ekran uygulama tanımı
- `sw.js` — kontrollü offline/cache katmanı
- `icon-*.png` — LAGORA uygulama ikonları
- `.nojekyll` — GitHub Pages'de dosyaların olduğu gibi servis edilmesi için

## Veri korunumu
Mevcut veri blokları bu pakette değiştirilmedi:
- `PRODUCTS`: 654
- `FRAGRANCE_META`: 419
- `META_ALIASES`: 248

## GitHub Pages kurulumu
1. GitHub'da yeni bir repository aç.
2. Bu klasördeki **dosyaların tamamını** repository'nin köküne yükle. ZIP dosyasını tek başına yükleme; ZIP'i açıp içindeki dosyaları yükle.
3. Repository → **Settings → Pages**.
4. **Build and deployment → Source: Deploy from a branch** seç.
5. Branch olarak `main`, folder olarak `/ (root)` seçip Save de.
6. GitHub'ın verdiği `https://KULLANICI.github.io/REPO/` adresini WhatsApp grubuna gönder.

GitHub Pages statik HTML/CSS/JavaScript dosyalarını doğrudan repository'den yayınlayabilir. `index.html` giriş dosyası olarak kullanılır. Yayın sonrası HTTPS desteklenir.

## iPhone
Linki **Safari** ile aç. Ardından **Paylaş → Ana Ekrana Ekle → Web Uygulaması olarak aç** seçeneğini kullan. Böylece LAGORA bir uygulama gibi açılır.

## Güncelleme
Yeni `index.html` yüklediğinizde service worker yeni sayfayı ağdan almaya çalışır ve son başarılı sürümü cache'e yazar.

## Önemli
GitHub Pages üzerindeki site internete açık olabilir. Ticari olarak gizli kabul ettiğiniz veri varsa yayınlama politikanızı kontrol edin.
