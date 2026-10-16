JARVIS Android

Gemini Live tabanlı sesli asistan (V3'ün Android karşılığı). Kendi ücretsiz Gemini API anahtarınla çalışır.

## Derleme
1. Android Studio (Koala veya yeni) ile bu klasörü aç → Gradle sync (wrapper'ı kendisi oluşturur).
2. Telefonu USB ile bağla (geliştirici modu) → Run.
3. Uygulamada ⚙ → API anahtarını yapıştır (https://aistudio.google.com/apikey) → Kaydet → mikrofon düğmesine dokun.

APK için: Build → Build Bundle(s)/APK(s) → Build APK(s).

## Özellikler
Sesli sohbet (sözünü kesebilirsin), yazılı mesaj, kalıcı hafıza, uygulama açma, hava durumu, pil/saat,
Google/YouTube/Spotify arama-açma, medya kontrolü, takvim etkinliği, alarm, WhatsApp mesaj hazırlama.

## Notlar
- Model adı ⚙ ayarlarından değiştirilebilir (varsayılan: gemini-2.5-flash-native-audio-latest;
  alternatif: gemini-3.1-flash-live-preview).
- Android, WhatsApp mesajını ve takvim kaydını kullanıcı onayı olmadan göndermeye izin vermez; uygulama ilgili ekranı açar.
- Uygulama arka plana geçince mikrofon oturumu kapanır (Android kısıtı).

## Android Studio olmadan APK (GitHub ile)
1. Bu klasörün içeriğini yeni bir GitHub deposuna yükle (ZIP'in içindekiler depo kökünde olmalı).
2. Depoda Actions sekmesi → "APK derle" → çalışmasını bekle (~5 dk).
3. Çalışmanın altındaki "JARVIS-apk" dosyasını indir, zip'ten `app-debug.apk` çıkar, telefona at ve kur
   (Ayarlar'dan "bilinmeyen kaynaklardan yüklemeye izin ver").
