# StreamFlow TV - Samsung Tizen IPTV Player

## Özellikler
- 📺 M3U/M3U8 URL ve dosya desteği
- 🎬 VOD (isteğe bağlı içerik) görünümü
- 📡 Kanal grupları ve filtreleme
- 🔍 Anlık arama (canlı + VOD)
- 📱 Samsung uzaktan kumanda tam desteği
- ⚡ HLS.js ile gelişmiş stream desteği
- 💾 Son kanal ve kaynak hatırlama

## Kurulum (Samsung Tizen)

### Yöntem 1 – Tizen Studio (Geliştirici)
1. Tizen Studio'yu bilgisayara kur
2. TV'de Geliştirici Modunu aç: `Ayarlar > Destek > Tizen Geliştirici Modu`
3. TV IP adresini gir
4. Tizen Studio'da "Import Project" > bu klasörü seç
5. Run > Run As > Tizen Web Application

### Yöntem 2 – USB Sideload (Bazı TV modelleri)
1. `index.html` ve `config.xml` dosyalarını USB'ye kopyala
2. USB'yi TV'ye tak
3. Dosya yöneticisinden `index.html` dosyasını aç

### Yöntem 3 – Web Server (Tavsiye Edilen)
1. Dosyaları bir web sunucusuna yükle (GitHub Pages ücretsiz)
2. TV'nin tarayıcısını aç
3. URL'yi gir

## Uzaktan Kumanda Kısayolları
| Tuş | Fonksiyon |
|-----|-----------|
| ▲▼ | Kanal değiştir |
| ENTER | OSD göster |
| BACK | Geri |
| MUTE | Ses kapat/aç |
| INFO | Kanal bilgisi |
| 🔴 Kırmızı | VOD görünümü |
| 🔵 Mavi | Canlı TV |
| 🟢 Yeşil | Arama |
| 🟡 Sarı | M3U ekle |

## M3U Kullanımı
1. "KAYNAK EKLE" sekmesine git
2. M3U URL'nizi girin (örnek: `http://yourprovider.com/playlist.m3u`)
3. "YÜKLE" butonuna bas
4. Kanallar otomatik yüklenir

## Notlar
- CORS kısıtlaması olan M3U URL'leri için proxy kullanılır
- HLS (.m3u8) stream'ler otomatik algılanır
- localStorage ile son kanal ve kaynaklar hatırlanır
