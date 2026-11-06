# Music — iOS öncelikli web uygulaması

Bu depodaki tüm dosyalar tek dizindedir. `assets` gibi alt klasör oluşturmanız gerekmez.

## GitHub Pages ile yayınlama

1. Bu paketteki dosyaların tamamını GitHub deposunun ana dizinine (root) yükleyin. `index.html` doğrudan ana dizinde bulunmalıdır.
2. GitHub deposunda **Settings → Pages** bölümünü açın.
3. **Deploy from a branch** seçin; `main` dalını ve `/(root)` klasörünü seçip kaydedin.
4. GitHub Pages adresiniz HTTPS üzerinden yayınlandığında uygulama ve service worker çalışır.

## iPhone / iPad ana ekrana ekleme

1. Yayınlanan adresi **Safari** ile açın.
2. Paylaş düğmesine dokunun.
3. **Ana Ekrana Ekle** seçeneğini seçin. Varsa **Web Uygulaması Olarak Aç** seçeneğini açık bırakın.
4. Ekle'ye dokunun. iOS ana ekran simgesi `apple-touch-icon.png` dosyasından gelir.

## Dosyalar (tamamı kök dizinde)

- `index.html` — uygulama
- `apple-touch-icon.png` — iOS ana ekran simgesi (180×180)
- `icon-192.png`, `icon-512.png` — PWA simgeleri
- `favicon.ico`, `favicon-16.png`, `favicon-32.png` — tarayıcı simgeleri
- `manifest.webmanifest` — uygulama adı, simgeler ve görüntüleme ayarları
- `service-worker.js` — uygulama kabuğu önbelleği

**Not:** GitHub'a yüklerken dosyaları ZIP'in içinden çıkarıp doğrudan depo ana dizinine koyun; ZIP dosyasının kendisini yüklemeyin.
