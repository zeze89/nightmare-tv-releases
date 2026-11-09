# Nightmare TV: IPTV Kullanıcı Persona Araştırması (Birleşik Değerlendirme)

Tarih: 2026-11-09 · Yöntem: 9 persona simülasyonu (3 Fable, 3 Opus, 3 Sonnet; her modelde PC, TV, mobil)

> **Önemli uyarı:** Bu bir SİMÜLASYONDUR, gerçek arama hacmi veya analitik verisi değildir. Sorgu örnekleri, yüzdeler ve sıralamalar modellerin gerçekçi tahminleridir. Yalnızca 5 persona web araması yaptı (Fable x3, Opus mobil) ve bunlar sadece bağlamı doğruladı (aşağıda işaretli). Karar vermeden önce Search Console, Play Console / Microsoft Store / Samsung / LG arama terimi raporları, Google Trends ve gerçek kullanıcı görüşmeleriyle doğrulanmalı.

## 1. Personalar

| Model | PC | TV | Mobil |
|---|---|---|---|
| Fable | Emre, 34, TR, L2 destek, Windows | Mehmet, 52, DE, Samsung Tizen + Fire TV | Lucas, 22, BR, Android |
| Opus | Mark, 41, ABD, DevOps power user | Callum, 29, UK, Fire TV sideload | Dmitri, 38, RU expat TR'de, iPhone |
| Sonnet | Hasan, 58, TR, emekli, Edge/Bing | Mehmet K., 45, TR, LG webOS, çocuklu aile | Imran, 27, BAE, Pakistanlı, Android |

## 2. Platform bazlı arama alışkanlıkları (simüle)

| Platform | Gözlem | Tipik sorgu (örnek) |
|---|---|---|
| **Google** | Çoğu personada ana motor (TR, UK, BR, BAE). Sorun çözme ve "en iyi" araması. | `m3u link nasıl izlenir`, `iptv donuyor`, `best iptv player firestick reddit`, `melhor app iptv android` |
| **Bing** | Bilinçli seçilmiyor; Edge varsayılanı ve Copilot yüzünden dolaylı pay. DDG sonuçları Bing indeksine dayandığından önemli (Opus PC). | `iptv player microsoft store`, `m3u player windows 11` |
| **Yandex** | Rusça konuşanda ana motor (~%50 tahmin); diğerlerinde "Google'da çıkmayanı bul" ve gri içerik arayışı. Güvensiz algılanıyor. | `iptv плеер для iphone`, `ott navigator windows` |
| **DuckDuckGo** | Gizlilik odaklı power user'da ana motor; diğerlerinde "hassas" aramalar (yasallık, VPN, liste). | `iptv player no account no telemetry`, `is iptv legal turkey` |
| **YouTube** | Her personada kurulum ve güven doğrulama kanalı. Güncel (≤3 ay) ve yerel dilde video ağırlıklı. | `samsung tv iptv kurulumu`, `how to install iptv on firestick 2026` |
| **Mağazalar** | Play Store, Microsoft Store, LG/Samsung/Amazon mağazaları kısa terim aranıyor: `iptv`, `m3u player`, `xtream`, `smarters`. | `iptv`, `iptv player`, `m3u` |
| **Reddit / GitHub / forum** | Teknik personada en güvenilen kaynak. `reddit` kelimesi sorguya eklenerek SEO bloglarından kaçılıyor. | `tivimate alternative for pc`, `iptvnator issues` |
| **Telegram / WhatsApp / TikTok** | Mobil ve düşük teknik personalarda asıl keşif ve link kaynağı. Mağaza genelde son doğrulama adımı. | satıcı ve arkadaş tavsiyesi |

**Doğrulanan bağlam (web aramasıyla):** Samsung mağazasında IPTV Smarters Pro'nun görünmemesi ve Smart IPTV'nin 2019'da kaldırılması; Brezilya'da Anatel/Ancine IP bloklama baskısı; Apple'ın Rusya App Store'undan VPN uygulamalarını kaldırması; PC aramalarında IPTV satıcılarına bağlı SEO bloglarının baskınlığı. Doğrulanmayan: Fire TV'de Vega OS ve sideload kısıtı (ajanın kendi bilgisi).

## 3. En çok aranan temalar (9 personada ortak)

1. **Kurulum / kaynak ekleme:** "nasıl kurulur", "m3u nasıl eklenir", "xtream nedir" (9/9)
2. **Donma / buffering, özellikle maç anında** (9/9)
3. **"En iyi IPTV player" karşılaştırması ve TiviMate/Smarters alternatifi** (7/9)
4. **EPG sorunları:** gelmiyor, saat kayık, eşleşmiyor (7/9)
5. **Güven ve yasallık:** "güvenli mi", "yasal mı", "virüs var mı" (8/9)
6. **Spor yayını:** Süper Lig, Premier Lig, F1, kriket, Brasileirão (7/9)
7. **Kanal listesi karmaşası:** favori, filtre, dil/ülke ayrımı (8/9)
8. **Cast / PiP:** Chromecast, AirPlay, arka planda izleme (mobil personaların hepsi)
9. **Catch-up / timeshift / kayıt** (5/9)
10. **Ücretsiz / reklamsız / tek seferlik ödeme** (7/9)

## 4. Ortak ihtiyaçlar ve acı noktaları

1. **İlk 5 dakika kurulum duvarı.** TV'de kumandayla URL yazmak, PC'de nereye yapıştıracağını bilmemek, mobilde M3U/Xtream karışıklığı. En çok terk edilen nokta.
2. **Donma ve "suçlu kim?" belirsizliği.** Kullanıcı sorunun uygulamadan mı, sağlayıcıdan mı, internetten mi geldiğini ayırt edemiyor ve uygulamayı siliyor.
3. **Güven.** İçerik satan, reklamlı, izinleri fazla ya da kaynağı belirsiz uygulama hepsinde deal-breaker.
4. **Büyük listelerde gezinme** (5-15 bin kanal): ülke/dil filtresi, favori, grup gizleme.
5. **Cihaza özgü kısıtlar:** TV'de düşük RAM ve mağaza kısıtı, mobilde veri kotası ve pil, PC'de zayıf rakip ve güven.

## 5. İstenen özellikler (öncelikli)

**Must-have (hemen hemen tüm personalar)**
- Xtream Codes + M3U + XMLTV EPG, çoklu playlist, yedek kaynağa geçiş
- QR / telefon eşleştirme / panodan otomatik algılama ile kolay kurulum
- Hızlı kanal geçişi, güçlü arama, favoriler, kategori/dil filtresi
- Otomatik yeniden bağlanma, ayarlanabilir buffer, anlaşılır hata mesajı ("sunucu çevrimdışı", "abonelik bitti")
- Yerel dil arayüz (TR, DE, pt-BR, RU, EN) ve büyük yazı seçeneği
- EPG saat dilimine duyarlı
- Reklamsız çekirdek, hesap zorunluluğu yok, telemetri yok ya da kapatılabilir

**Cihaza özgü must-have**
- PC: klavye kısayolları, rakamla kanal, mini pencere "her zaman üstte", çoklu monitör hafızası, imzalı kurulum, donanım hızlandırma
- TV: Tizen/webOS/Fire TV/Android TV mağaza varlığı, rakam tuşlarıyla geçiş, hafif çalışma, çocuk kilidi
- Mobil: gerçek PiP, arka plan ses, Chromecast ve AirPlay, hücresel veride düşük kalite ve veri sayacı, ağ değişiminde kesintisiz toparlanma

**Nice-to-have:** multiview, catch-up/timeshift, DVR, maç hatırlatma bildirimi, TMDB posterli VOD, bağlantı tanı paneli, ayar yedekleme/senkron, çoklu profil, portable/winget/Flatpak paketleri.

**Deal-breaker:** içerik veya abonelik satmak, zorunlu hesap/kart, tam ekran reklam, imzasız ya da kaynağı belirsiz binary, zorunlu aylık abonelik, yalnızca İngilizce arayüz, sık çökme.

## 6. Model karşılaştırması (persona üretim farkları)

- **Fable:** En somut. Persona'ya özgü kaynaklı doğrulama yaptı (4 ajanda 3-4 arama), mağaza/Tizen/Fire TV kısıtlarını ve "TV'de arama aslında telefonda olur" içgörüsünü çıkardı. Tüm Fable ajanları kaynak sundu, ama kaynakların çoğu satıcı/SEO sayfası.
- **Opus:** En stratejik. Dağıtım riski (Vega OS, Apple ID bölgesi), konumlandırma ve gizlilik odaklı güven kriterlerini öne çıkardı. Opus PC ve TV web araması yapmadı; yalnızca mobil yaptı.
- **Sonnet:** En kullanıcı-yakın ve pratik. Düşük teknik seviyeyi (Edge/Bing, mağaza güveni, kumanda sorunu, çocuk güvenliği) en iyi yansıtan model; hiçbir Sonnet ajanı web araması yapmadı.
- **Not:** Persona tanımları modele göre farklı olduğundan, farklar "model farkı" mı "persona farkı" mı net ayrılamaz. Temiz bir model karşılaştırması için aynı persona'yı üç modelde çalıştırmak gerekir.

## 7. Ek değerlendirme kriterleri (benim eklediklerim)

| Kriter | Değerlendirme |
|---|---|
| **Yasal / itibar riski** | Her personada "içerik satmayan sadece player" konumlandırması güveni artırıyor. Kaçak içerik çağrışımı mağaza reddi ve marka riski yaratır. Hukuki görüş alınmalı. |
| **Marka adı** | "Nightmare" üç ayrı persona (Opus TV, Sonnet TV, Fable TV) tarafından olası güven/aile engeli olarak işaretlendi: sesli arama yanlış tanıma, çocuklu ev çağrışımı, Almanca "Albtraum". Gerçek kullanıcılarla test edilmeli. |
| **Mağaza SEO / keşfedilebilirlik** | Kısa terimler (`iptv`, `m3u`, `xtream`, `smarters`) mağaza başlık ve anahtar kelimelerine girmeli. Uzun kuyruklu sorunlar ("iptv donuyor", "m3u nasıl izlenir") yerel dilde YouTube/blog içeriğiyle yakalanmalı. |
| **Kurulum sürtünmesi** | Tüm cihazlarda dönüşümü belirleyen metrik. İlk açılıştan ilk oynatmaya süre (hedef <2 dk) ve QR/kod eşleştirme başarı oranı izlenmeli. |
| **Dağıtım kırılganlığı** | TV'de mağaza varlığı kritik (Tizen'de sideload yok). Fire TV'de sideload kısıtı konusu doğrulanmalı. iOS'ta bölge Apple ID'leri. |
| **Gelir modeli** | Tek seferlik / lifetime tercih ediliyor (R$15-30, ~$20-30 power user); aylık abonelik kullanıcının sağlayıcı ücretiyle yarışıyor. Reklam çoğu persona için deal-breaker. |
| **Farklılaşma** | PC'de "TiviMate kalitesinde masaüstü player" boşluğu; mobilde Chromecast+PiP+veri tasarrufu; TV'de QR kurulumu ve hafiflik. |
| **Yerelleştirme** | TR, DE, pt-BR, RU, Hint/Urdu dilleri personalara göre öne çıkıyor. Pazar önceliği analitikle belirlenmeli. |
| **Destek / güven kanalları** | Telegram/WhatsApp topluluğu, Reddit'te şeffaf geliştirici, GitHub release + changelog; yerel dilde kısa kurulum videosu. |

## 8. Önerilen öncelik sırası

1. İlk açılış ve eşleştirme akışı (QR, kod, pano algılama, yerel dil rehber)
2. Güvenilirlik: otomatik yeniden bağlanma, net hata mesajları, bağlantı tanı göstergesi
3. Güven paketi: "içerik sağlamıyoruz" konumu, imzalı paketler, telemetri yok sayfası, mağaza varlığı
4. EPG doğruluğu ve kanal gezinme (filtre, favori, hızlı zapping)
5. Cihaza özgü farklılaştırıcılar (PC masaüstü özellikleri, mobil PiP/cast/veri tasarrufu, TV hafiflik)
6. İçerik/SEO: kısa mağaza anahtar kelimeleri + yerel dilde sorun-çözüm içeriği
7. Marka adı testi ve yerelleştirme

## 9. Sonraki adım: gerçek veri ile doğrulama

- Google Search Console, Bing Webmaster Tools, Play Console / Microsoft Store arama terimi raporları
- Google Trends (TR, DE, BR, UK, BAE) ve mağaza anahtar kelime araçları
- Reddit (r/IPTV, r/firetv, r/selfhosted), Technopat/DonanımHaber başlık taraması
- 10-15 gerçek kullanıcıyla görüşme veya anket (özellikle marka adı ve kurulum akışı)
