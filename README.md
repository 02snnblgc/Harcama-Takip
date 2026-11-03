# Modüler Android Bütçe Takip Uygulaması (PWA)

Bu proje; tamamen çevrimdışı çalışabilen, `localStorage` veri tabanına sahip, özel simgeli (`assets/icon.png`), bütçe limit takibi, 3D gradyan arayüzü ve JSON yedekleme modüllerini içeren modern bir Progressive Web App (PWA) bütçe takip uygulamasıdır.

## Proje Dosya Yapısı
```text
/budget_app
│
├── index.html       # Ana uygulama arayüzü ve JavaScript mantığı
├── manifest.json    # PWA ve özel simge yapılandırması
└── assets/
    └── icon.png     # Uygulama simgesi
```

## GitHub Üzerinden APK'ya Dönüştürme Rehberi (PWA to APK)

Bu web uygulamasını telefonunuza yerel bir Android uygulaması (APK) olarak kurmak ve GitHub üzerinden otomatik paketlemek için aşağıdaki adımları takip edebilirsiniz:

1. **GitHub Repository Oluşturma:**
   - GitHub hesabınızda yeni bir public (açık) repository oluşturun (Örn: `budget-tracker-app`).
   - `budget_app` klasörü içindeki tüm dosyaları (`index.html`, `manifest.json`, `assets/icon.png`) bu repository'nin ana dizinine yükleyin.

2. **GitHub Pages Aktifleştirme:**
   - Repository ayarlarına (`Settings`) gidin.
   - Sol menüden `Pages` sekmesini seçin.
   - `Build and deployment` altında `Branch` kısmını `main` (veya `master`) olarak seçip `Save` deyin. Birkaç dakika sonra siteniz `https://kullaniciadi.github.io/budget-tracker-app/` adresinde yayına girecektir.

3. **APK Oluşturma (Bubblewrap / PWABuilder):**
   - [PWABuilder.com](https://www.pwabuilder.com/) adresine gidin.
   - Yayınlanan GitHub Pages URL'nizi (`https://...`) arama çubuğuna yapıştırıp `Start` butonuna basın.
   - Site uygulamanızı tarayacak ve PWA skorunu gösterecektir.
   - **"Generate Android App"** butonuna tıklayın.
   - Çıkan formda paket adını (Örn: `com.budget.tracker`) ve uygulama adını girerek **"Generate"** deyin.
   - Sistem sizin için hem imzalı APK dosyasını hem de Android Studio kaynak kodunu içeren bir ZIP paketi indirecektir. İndirdiğiniz APK'yı doğrudan telefonunuza kurabilirsiniz!
