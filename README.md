# Şirket Takvimi ve Günlük Rapor Arşivi

JavaFX ile geliştirilmiş haftalık takvim, kullanıcı bazlı etkinlik ve günlük rapor uygulamasının **derlenmiş dosya arşivi**. Depodaki sınıf imzaları takvim ve rapor işlemlerini gösterir; proje bir web raporlama arayüzü değildir.

## Mevcut dosyalar

| Dosya | İçerik |
| --- | --- |
| `Takvim.exe` | Windows çalıştırılabilir dosyası |
| `TakvimUygulamasi.class` | `com.rapor.TakvimUygulamasi` JavaFX uygulama sınıfı |
| `TakvimUygulamasi$ParsedEvent.class` | Etkinlik yardımcı sınıfı |
| `ReportService.class` | Tarihe ve kullanıcıya göre rapor okuma/yazma servisi |
| `style.css` | Arayüz stilleri |
| `module-info.class` | Arşivde bulunan modül tanımlayıcı dosya |

## Görülebilen işlevler

Derlenmiş sınıf metaverisi; kullanıcı seçimi, haftalık takvim, etkinlik ekleme/silme, günlük rapor yazma ve tarihe göre rapor görüntüleme metotlarını içerir. Bu, uygulamanın bu ortamda çalıştırıldığı anlamına gelmez.

## Çalıştırma ve geliştirme durumu

Windows paketinin giriş noktası `Takvim.exe` dosyasıdır. Gerekli Java/JavaFX çalışma zamanı veya yardımcı paketlerin tümünün bu repoda yer aldığı doğrulanmamıştır; dolayısıyla tek komutla kurulum/çalıştırma garantisi verilmez.

Java kaynak dosyaları, Maven/Gradle build tanımı ve otomatik testler depoda yoktur. `.class` dosyaları kökte dururken iç paket adları `com.rapor` olduğundan doğrudan `java TakvimUygulamasi` komutu uygun bir paketleme yolu değildir. Kaynaktan yeniden derleme için özgün `.java` dosyaları ve JavaFX bağımlılıkları eklenmelidir.

Bu repo mevcut çıktıları belgeleyen bir arşivdir; README güncellemesi çalıştırılabilir dosyayı yeniden üretmedi veya uygulamayı test etmedi.
