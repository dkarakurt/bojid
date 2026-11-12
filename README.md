# bojid-R

Tarayıcıda ve Android'de çalışan 8 kanallı synthesizer / groovebox.

- `web/index.html` — web sürümü (siteye tek dosya olarak yüklenir)
- `app/` — Android uygulaması (WebView, her zaman yatay açılır)

## APK

`main` dalına her push'ta GitHub Actions APK'yı derler ve **Releases** sayfasına `bojid-R.apk` olarak koyar.
Elle çalıştırmak için: Actions → Build APK → Run workflow.

Kurulum: APK'yı telefona indir, aç; "bilinmeyen kaynaklardan yükleme" izni istenirse ver.

## Web sürümünü güncellemek

`web/index.html` değiştiğinde aynı dosyayı `app/src/main/assets/index.html` üzerine kopyala ve push et.

## Yerel derleme

Android Studio → Open → bu klasör → Build → Build APK(s).
Ya da Android SDK + Gradle 8.9 ile: `gradle assembleRelease`
