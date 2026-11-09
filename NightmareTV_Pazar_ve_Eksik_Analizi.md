# Nightmare TV: Eksikler, Eklenecek Özellikler ve "Pazarda Tek Olma" Analizi

Tarih: 2026-11-09 · Kapsam: 3 sabit persona (PC, TV, mobil) × 3 model (Fable, Opus, Sonnet) = 9 simülasyon + 1 web tabanlı rakip analizi

## 0. Önce bilinmesi gerekenler (güvenilirlik)

- **Bu bir simülasyondur, gerçek kullanıcı verisi değildir.** Puanlar, fiyat aralıkları, arama sorguları ve "ilk tepki" modellerin tahminidir. Gerçek ölçüm için Search Console, Play Console ve mağaza arama raporları, gerçek kullanıcı görüşmeleri gerekir.
- **Ürün bilgisi yalnızca GitHub release notlarından (v2.1.79 → v2.2.6) çıkarıldı.** nightmaretv.net bu ortamdan erişilemedi. Bu yüzden aşağıdaki "eksik" maddelerinin çoğu aslında **"release notlarında geçmiyor"** demektir. Ürününüzde zaten varsa bunlar eksik değil, **iletişim/keşif eksiğidir** (ki bu da bir bulgudur). Her maddeyi kendi ürününüze karşı işaretleyin (bölüm 9).
- **Web doğrulaması:** 6 persona ajanı arama yaptı (Fable x3, Opus x3), Sonnet x3 yapmadı. Rakip analizi 39 arama/okuma yaptı. Rakip kaynaklarının çoğu IPTV satıcılarının SEO sayfalarıdır; fiyatlar "yaklaşık/çelişkili" okunmalı. Reddit'e erişilemedi. TorrentFreak ve AFTVnews yalnızca arama özetinden okundu.
- **Kontrollü deney:** Aynı 3 persona, aynı prompt, aynı ürün bilgi notu, 3 modelde çalıştırıldı. Üç model aynı model ailesinden geldiği için örtüşmeleri bağımsız doğrulama sayılmaz.

## 1. Yönetici özeti

1. **Ürün güçlü, ama kimse bilmiyor.** Teknik derinlik (akıcılık, teşhis, şeffaflık) rakiplerden ileride görünüyor. Puan ortalaması: bağlılık 6.9, kurulum 6.1, ama **keşfedilebilirlik 3.0, güven 4.2, ödeme isteği 4.7**. Sorun ürün kalitesinden çok **görünürlük, güven ve ticari netlik**.
2. **PC'de iş neredeyse hazır, TV ve mobilde değil.** PC personasının tavsiye puanı 6, TV ve mobilde 4-5. PC'de ürün pazar boşluğuna giriyor; TV'de Tizen/webOS yok ve kumandayla kurulum zor; mobilde cast ve veri kontrolü eksik (notlarda geçmiyor).
3. **Dokuz personanın dokuzu da aynı üç şeyi söyledi:** fiyat/deneme şeffaflığı yok, "Nightmare" adı sorun, gizlilik politikası/kod imzası belirsiz.
4. **"Pazarda tek" iddiası kısmen savunulabilir:** Android TV + Windows + Mac'te aynı ürün ve bulut senkron kombinasyonu rakip taramasında bulunamadı (kanıt: güçlü/orta). Glass Ledger, Best copy, Missed seconds gibi özellikler rakiplerde bulunamadı ama "yokluk kanıtı" doğası gereği zayıf.
5. **En büyük dış risk mağaza kaldırması.** 2026'da "yalnızca player" olmak Google Play'den toplu kaldırmayı engellemedi (JioStar/Delhi Yüksek Mahkemesi, Mart 2026, 36 uygulama; XCIPTV, Televizo, Smarters dahil). Microsoft Store için kaldırma haberi bulunamadı: MSIX sürümü stratejik avantaj.

## 2. Ürünün release notlarından görünen profili

- **Platformlar:** Windows (Setup, Portable, MSIX/Store), macOS (.dmg), Android telefon/tablet/Android TV (arm64, armv7, x86_64, universal APK; Google Play).
- **Geçmeyenler:** iOS, Apple TV, Samsung Tizen, LG webOS, Linux, tarayıcı, Fire TV (açıkça).
- **Güçlü yönler:** Xtream + M3U + harici XMLTV, deinterlacing/50 fps/refresh rate eşleme, Best copy, Smoothness Report, kanal açılmazsa neden gösterme ve Xtream hesap teşhisi, catch-up, kayıt, Multi-view, Missed seconds, Home channels, Home Tower preview, PIN ile ebeveyn kontrolü (her yerde), profiller, şifreli Cloud Sync, Glass Ledger (uygulamanın ağ isteklerinin canlı listesi), 10 arayüz dili, doğal dil rehber araması.
- **Gerçek görünürlük (Fable PC web aramasıyla):** AlternativeTo (TiviMate alternatifleri dahil), Softpedia, winget (`NightmareTv.NightmareTV`), Microsoft Store ve DonanımHaber'de geliştiricinin kendi tanıtım başlığı ("libmpv IPTV oynatıcı, Win/Android TV/macOS"). Opus PC AlternativeTo'yu bağımsız buldu. Bu, PC kanallarında görünürlüğün sıfır olmadığını gösteriyor. **TV ve satıcı kanallarında ise iz bulunamadı** (Fable TV, Opus mobil, Fable mobil aramaları).
- **Web listelerinde geçen ama bilgi notunda olmayan (doğrulanmadı):** 14 gün deneme, HDR tone-mapping, Fire TV desteği. Ürün sahibi doğrulamalı. Ayrıca web listelerinde sürüm numaraları tutarsız (2.1.88 / 2.1.99 / 2.2.3), "bakımsız mı?" algısı yaratabilir.

## 3. Puan tablosu (1-10, persona × model)

| Persona | Model | Keşif | Kurulum | İlk 5 dk | Güven | Bağlılık | Ödeme | Öneri |
|---|---|---|---|---|---|---|---|---|
| PC (Emre) | Sonnet | 3 | 7 | 7 | 4 | 8 | 6 | 6 |
| PC | Opus | 4 | 7 | 7 | 4 | 8 | 6 | 6 |
| PC | Fable | 5 | 8 | 6-7 | 6 | 7 | 6 | 6 |
| TV (Murat) | Sonnet | 3 | 5 | 6 | 4 | 7 | 5 | 5 |
| TV | Opus | 2 | 5 | 6 | 4 | 7 | 4 | 4 |
| TV | Fable | 2 | 4 | 6 | 4 | 7 | 4 | 4 |
| Mobil (Cem) | Sonnet | 3 | 6 | 6 | 4 | 6 | 4 | 4 |
| Mobil | Opus | 3 | 7 | 6 | 4 | 6 | 4 | 5 |
| Mobil | Fable | 2 | 6 | 6 | 4 | 6 | 3 | 4 |
| **Ortalama** | | **3.0** | **6.1** | **6.3** | **4.2** | **6.9** | **4.7** | **4.9** |

**Cihaza göre ortalama:** PC (keşif 4.0, kurulum 7.3, öneri 6.0) · TV (keşif 2.3, kurulum 4.7, öneri 4.3) · Mobil (keşif 2.7, kurulum 6.3, öneri 4.3).
**Modele göre ortalama:** Sonnet, Opus ve Fable keşif puanında aynı (3.0). Tavsiyede Sonnet 5.0, Opus 5.0, Fable 4.7. Ödeme isteğinde Sonnet 5.0, Opus 4.7, Fable 4.3. Modeller arası fark küçük; asıl fark persona (cihaz) farkı.

## 4. Eksikler: kaç persona söyledi ve ne kadar kritik

"Release notlarında geçmiyor" = doğrulanmalı. Sıklık 9 personadan kaçının ilgili maddeyi işaretlediğini gösterir.

| # | Madde | Sıklık | En kritik olduğu cihaz | Etki |
|---|---|---|---|---|
| 1 | **Fiyat, lisans kapsamı ve deneme süresinin şeffaflığı** (deneme sonrası Canlı TV kilitleniyor, tutar notlarda yok) | 9/9 | Hepsi | Kritik |
| 2 | **Marka adı "Nightmare"** (kâbus çağrışımı, aile TV'sinde red, arama sonuçlarında korku içerikleriyle karışma) | 9/9 | TV, mobil | Kritik (güven/keşif) |
| 3 | **Gizlilik politikası, telemetri ayrıntısı, kod imzası, yayıncı kimliği** | 9/9 | PC (Windows SmartScreen) | Kritik |
| 4 | **Kurulum: QR / telefondan eşleştirme / pano veya paylaş menüsünden içe aktarma** | 6/9 (TV ve mobil 6/6) | TV | Kritik (TV), yüksek (mobil) |
| 5 | **Chromecast / AirPlay / DLNA** | 9/9 anıldı, öncelik cihaza göre | Mobil (kritik), PC ve TV (orta) | Kritik (mobil) |
| 6 | **Mobil veri kontrolü** (hücresel kalite kilidi, veri sayacı, "bu maç ~X GB") | 3/3 mobil | Mobil | Kritik |
| 7 | **Tizen / webOS desteği** | 3/3 TV | TV | Kritik (aile tek uygulama ister) |
| 8 | **Kanal yönetimi** (ülke/dil/grup gizleme, sıralama, çift kayıt, logo) | 8/9 | PC, mobil | Yüksek-kritik |
| 9 | **Çocuk modu** (PIN var; "yalnızca çizgi film", süre sınırı yok) | 3/3 TV | TV | Yüksek |
| 10 | **Maç/kanal hatırlatma bildirimi** (reminders var, kapsamı belirsiz) | 8/9 | Mobil | Yüksek |
| 11 | **Telefonda PiP ve arka planda yalnızca ses** | 3/3 mobil | Mobil | Yüksek |
| 12 | **Çok cihazlı aile lisansı** | 6/9 | TV | Yüksek |
| 13 | **Windows'ta anlık kayıt belirsizliği, harici oynatıcı, User-Agent/header ayarı, ham log/codec paneli, klavye kısayolları / 10-foot UI** | PC 3/3 | PC | Yüksek |
| 14 | **TMDB poster/metadata** | 9/9 anıldı | Mobil, TV | Orta |
| 15 | **Satıcı ekosistemi: MAC/cihaz kodu ile portal aktivasyonu; Play'de TV listelemesi** | Fable TV | TV (Türkiye) | Yüksek (Fable TV'ye özgü) |
| 16 | **Kaynak kodu kapalı** (repo yalnızca installer dağıtıyor) | PC 3/3 | PC (teknik) | Orta |
| 17 | **Xtream + yedek M3U otomatik failover** | Fable PC | PC | Orta |
| 18 | **Türkçe kurulum videosu, yardım içeriği, topluluk kanalı** | TV 3/3 | TV | Yüksek (keşif) |
| 19 | **Güncelleme kanalı karışıklığı** (Setup / Portable / MSIX farklı kanallar) | Fable PC | PC | Orta |
| 20 | iOS, Linux, Fire TV net destek bilgisi | 3-5/9 | Değişken | Orta |

## 5. Eklenmesi gereken özellikler: öncelikli yol haritası

### Önce doğrula (yazılım yazmadan)
Bölüm 4'teki maddelerin hangisi üründe zaten var? Varsa mağaza metni, ekran görüntüleri ve web sitesi bunu anlatmalı. Özellikle: Chromecast, telefonda PiP, QR/pano, veri sayacı, çocuk modu, çok cihaz lisansı, kayıt kapsamı, Play'de TV listelemesi, deneme süresi.

### P0: 0-30 gün (güven ve ticari netlik, düşük kod, yüksek etki)
1. **Fiyat, deneme ve lisans kapsamı:** Mağaza ve web sitesinde net: deneme gün sayısı, tek seferlik/yıllık fiyat (TL dahil), kaç cihaz. Tüm personalar en az 14 gün deneme istedi. Deneme bitince Canlı TV'nin ani kilitlenmesi yerine uyarı ve tolerans süresi.
2. **Güven paketi:** Yazılı gizlilik politikası, Windows kod imzası (EV), SHA256 (zaten SHA256SUMS.txt var), "uygulama içerik sağlamaz, liste/kanal içermez" beyanı, Glass Ledger'ın tek sayfalık anlatımı. Glass Ledger'da görülebilecek her ağ isteği açıklanabilir olmalı (PC persona tek açıklanamayan isteği silme nedeni saydı).
3. **Marka algısı:** Mağaza başlığına açıklayıcı alt başlık ("Nightmare TV: IPTV Player, Xtream & M3U"), ikon ve ekran görüntüleri korku çağrışımını yumuşatsın. İsim değişikliği kararı için gerçek kullanıcı testi (bölüm 7).
4. **Mağaza SEO ve sürüm tutarlılığı:** Kısa terimler (`iptv`, `m3u`, `xtream`) başlık/anahtar kelimelerde; web listelerindeki tutarsız sürüm numaralarını düzelt (AlternativeTo, Softpedia, winget).
5. **Türkçe kısa kurulum videosu** (2-3 dk, Mi Box ve Windows) ve DonanımHaber/Technopat başlıklarını canlı tut.

### P1: 1-3 ay (kurulum sürtünmesi ve mobil eksikleri)
6. **QR / kısa kod / pano algılama / "paylaş ile aç" ile kurulum:** TV'de QR göster, telefondan Xtream/M3U bilgisini yapıştır veya paylaş menüsünden gönder. Bu, TV personalarının terk noktası (6/6).
7. **Mobil:** Cast (Chromecast, iOS sürümü varsa AirPlay), hücresel kalite kilidi + veri sayacı + "Wi-Fi'da HD, hücreselde düşük" varsayılanı, telefonda PiP ve ekran kapalı ses, ağ değişiminde (Wi-Fi→LTE) kesintisiz toparlanma.
8. **Kanal yönetimi:** Ülke/dil/grup gizleme, yeniden sıralama, çift kayıt birleştirme, EPG eşleştirme sihirbazı ve eşleşmeyenler raporu.
9. **Çocuk modu:** Yalnızca seçili kategoriler, günlük süre sınırı, PIN ile çıkış. Altyapı (PIN, profil) zaten var.
10. **Çok cihaz lisansı:** Hesap başı en az 3 cihaz (Windows + Android TV + telefon).
11. **Hatırlatma bildirimi:** Telefonda push, Windows'ta işletim sistemi bildirimi (e-posta alanı TV'de işe yaramıyor).

### P2: 3-6 ay (farklılaşma)
12. **Sağlayıcı/liste sağlığı paneli:** Hesap bitiş tarihi, aktif/maks bağlantı, gecikme, kopma geçmişi, dışa aktarılabilir teşhis raporu (kişisel veri temizli). **Dikkat:** Sağlayıcıya yönelik "karne" fikri hukuki/ticari risk taşır; önce teşhis, sonra paylaşım.
13. **Failover:** Ana Xtream düşünce yedeğe otomatik geçiş.
14. **Spor/Maç günü modu:** Best copy + Multi-view + Missed seconds + hatırlatma tek ekranda.
15. **PC için 10-foot UI ve klavye/gamepad:** HDMI ile TV'ye bağlanınca otomatik; kısayol listesi; harici oynatıcıya gönder, özel User-Agent/header, ham log ve codec/bitrate paneli.
16. **Tizen/webOS "eşlik" uygulaması veya cast tabanlı çözüm:** Tam sürüm yerine aynı lisans, aynı favori/profil/PIN. Not: Tizen/webOS mağazaları risk taşıyor (bölüm 7).
17. Windows anlık kayıt, TMDB posterleri, Linux, iOS (rakip kalabalık; en düşük öncelik).

## 6. "Pazarda tek olmak": hangi iddialar savunulabilir?

Rakip analizi 18 uygulamayı taradı (TiviMate, Smarters Pro, IBO, OTT Navigator, Televizo, XCIPTV, Smart IPTV, SS IPTV, GSE, Perfect Player, iptvnator, Hypnotix, Kodi, VLC, Jellyfin, Plex, MyIPTV, UHF/iPlayTV).

| # | İddia | Kanıt gücü | Not |
|---|---|---|---|
| 1 | **Android TV + Windows + Mac'te aynı ürün, sunucusuz bulut senkron + Home Tower:** bu kombinasyonu sunan başka bir ticari player bulunamadı | **Güçlü/orta** | TiviMate yalnızca Android TV; iptvnator yalnızca masaüstü; Jellyfin/Plex sunucu kurulumu ister. "Hiç yok" demek için mağazaların tam taraması gerekir. |
| 2 | **Glass Ledger:** uygulamanın kendi ağ trafiğini canlı listeleyen tek IPTV player | **Orta** | Rakiplerde yalnızca politika metni; IBO'nun gizlilik beyanları çelişkili. Yokluk kanıtı doğası gereği zayıf. |
| 3 | **Uygulama içi akıcılık çözümü** (deinterlacing, 50 fps hizalama, Best copy, Smoothness Report) | **Orta** | TiviMate deinterlacing'i işletim sistemine bırakıyor (destek yanıtı); Android TV 14'te 1080i→25 fps sorunu forumlarda belgeli. Nightmare'in bunu hangi platformlarda çözdüğü doğrulanmalı. |
| 4 | **Sağlayıcı/hesap kaynaklı hata teşhisi** (süre bitti / hesap kapalı / bağlantı dolu) | **Orta/zayıf** | Rakiplerde eşdeğeri bulunamadı ama mağaza açıklamaları tek tek incelenmedi. |
| 5 | **Missed seconds, Home channels** | **Zayıf/orta** | Niş; kullanıcı değeri doğrulanmadı. |

**"Tek biziz" denemeyecekler:** Ebeveyn kilidi, kayıt ve Multi-view rakiplerde yaygın. QR, Chromecast/AirPlay, iOS, Tizen/webOS, Linux ve Fire TV notlarda geçmiyor.

**Önerilen konumlandırma:** "Android TV'den Windows ve Mac'e, tek lisansla, kendi ağ trafiğini gösteren şeffaf IPTV oynatıcı." PC'de "TiviMate'in masaüstü karşılığı" mesajı en düşük maliyetli ve kanıtı en güçlü hamle (Windows'ta yerel TiviMate yok, emülatör öneriliyor; kanıt: kullanıcı forumları ve rehber siteleri).

## 7. Riskler

### Marka adı (9/9 persona işaretledi)
"Nightmare" Türkçe "kâbus"; aile TV'sinde çocuk ve eş itirazı, Almanca "Albtraum", arama sonuçlarında korku içerikleriyle karışma, ses aramada yanlış tanıma, bazı personalar için "malware adı". PC/teknik kullanıcıda etki daha hafif (Store, winget ve açıklayıcı alt başlık güveni toparlıyor). **Karar için:** 10-15 gerçek kullanıcıyla isim ve ikon testi, mağaza alt başlığı A/B. İsim değişikliği yerine önce açıklayıcı alt başlık ve görsel kimlik denenebilir.

### Dağıtım ve yasal (rakip analizinden)
- **Google Play:** 2019'dan beri tekrarlanan kaldırmalar (Smarters, Perfect Player); Mart 2026'da Hindistan'da 36 uygulama toplu kaldırıldı (XCIPTV, Televizo, Smarters Pro dahil). "Yalnızca player" itirazlarda işe yarıyor ama kaldırmayı engellemiyor, büyük spor turnuvalarında risk artıyor.
- **Amazon:** Korsan olarak tespit ettiği uygulamaları paket adına bakarak Fire TV'de devre dışı bırakıyor (AFTVnews). TiviMate Amazon mağazasında yok.
- **Microsoft Store:** IPTV player kaldırma haberi bulunamadı; MSIX sürümü düşük riskli kanal.
- **Samsung/LG:** SS IPTV'nin uyarısız kaldırıldığı geliştirici beyanı; Smart IPTV açıklamalarını "liste sağlamıyoruz" diye yeniden yazdı. Tizen/webOS'a girmek mağaza riski taşır. "Samsung/LG IPTV'yi AI ile engelliyor" iddiaları kaynaksız SEO yazıları, doğrulanamadı.
- **Risk azaltma (öneri):** Uygulama içinde hiçbir sağlayıcı tanıtmamak, örnek canlı liste koymamak, bayi/satıcı paneli olmamak, varsayılan listesiz açılmak, şeffaflık özelliklerini mağaza incelemesinde kanıt olarak sunmak. Bu adımların mağaza kabulüne etkisi kanıtlanmadı.
- **Pazarlama uyarısı:** Personalar Telegram/WhatsApp satıcı gruplarını keşif kanalı olarak gösterdi. Bu kanallara yönelik pazarlama, korsan IPTV ekosistemiyle ilişkilendirme riski taşır; mağaza ve yasal algıyı zedeler. Tavsiye: kanalları nötr tutmak (YouTube kurulum videoları, Reddit/forum, DonanımHaber, Store SEO), "bedava maç" ve lig/kulüp logosu söylemlerinden kaçınmak. Hukuki görüş alınmalı; bu rapor hukuki değerlendirme değildir.

### Satıcı ekosistemi (Türkiye)
Satıcılar "MAC gönder, IBO/Smarters kur" modelini ittiği için kullanıcı satıcının önerdiği uygulamayı kuruyor (Fable TV). Nightmare TV bu ağın dışında kalırsa TV segmentinde keşif zor. Çözüm yolu: aktivasyon modeli doğrulaması ve nötr, kural dışı olmayan ortaklık modeli (hukuki görüşle).

## 8. Fiyat ve lisans

- **Personaların ortak görüşü (9/9):** Tek seferlik "ömür boyu" lisans tercih, aylık abonelik reddi (IPTV listesine zaten aylık ödüyorlar), reklam kabul edilmez (güven ve çocuk gerekçesi), deneme **en az 7, tercihen 14 gün** (bir Süper Lig haftası ve bir hafta sonu maç döngüsünü kapsamalı), deneme bitince ani kilitlenme olmamalı.
- **Persona tahminleri (simülasyon):** Tek seferlik PC için 15-25 USD (500-900 TL), mobil/TV için 150-600 TL; yıllık 8-12 USD. Bu tutarlar persona tahminidir.
- **Rakip referansları (kalitesi değişken kaynaklar):** TiviMate yıllık ~5-10 $, ömür boyu ~20-40 $ (resmi fiyat doğrulanamadı; yıllık ücret 6.49→9.49 $ artışına tepki var; bir yorumcu ömür boyu seçeneğin kalktığını söylüyor). OTT Navigator ömür boyu 19.99 $. IBO Player cihaz başına tek seferlik 6-20 $. GSE iOS 2.99 $. Açık kaynak seçenekler ücretsiz.
- **Kullanıcıların kabul ettiği aralık (çıkarım):** Tek sefer 5-25 $, yıllık 5-12 $, aylık 1-2 $. Bu bandın üstü riskli.
- **Öneri:** Tek seferlik lisans + 14 gün tam özellikli deneme; hesap başı 3+ cihaz; Cloud Sync için isteğe bağlı küçük yıllık ücret düşünülebilir (PC persona); TL fiyatı Play/Store'da bölgesel. M3U'da sınırsız ücretsiz, Xtream'de premium ayrımı Fable mobil personanın fikri; ticari etkisi test edilmeli.

## 9. Ürün sahibi için doğrulama listesi

Aşağıdaki sorulara cevap verirseniz raporu "eksik" yerine "var/yok" olarak kesinleştirebilirim. Bunların çoğu release notlarında geçmiyor:

1. Chromecast/AirPlay/DLNA var mı?
2. Telefonda PiP ve arka planda ses var mı?
3. Hücresel veri kalite kilidi/sayacı var mı?
4. QR, kısa kod veya pano ile kurulum var mı?
5. Google Play'de Android TV cihazlarda listeleniyor mu (Mi Box S, Chromecast with Google TV)?
6. Fire TV'de çalışıyor mu, resmi desteğiniz var mı?
7. Deneme süresi gün sayısı ve fiyatlar nedir? Lisans kaç cihazı kapsıyor?
8. Gizlilik politikası, kod imzası, telemetri durumu nedir? Cloud Sync kapatılabilir mi, Xtream şifresi senkronize ediliyor mu?
9. Windows'ta anlık kayıt, klavye kısayolları, harici oynatıcı, özel User-Agent var mı?
10. Kanal filtreleme/gizleme/sıralama derinliği nedir? Kanal logosu ve ülke/dil gruplaması?
11. Çocuk modu (yalnızca seçili kategori, süre sınırı) var mı?
12. Hatırlatma bildirimleri hangi kanaldan (push, OS, e-posta) gider?
13. Listelenen 10 arayüz dili hangileri?
14. Web sitesi (nightmaretv.net) ve dokümanlarda hangi iddialar var? (Erişilemedi; içerik yapıştırırsanız ya da alan adına ağ izni verirseniz raporu güncelleyebilirim.)

## 10. Model karşılaştırması (aynı 3 persona, 3 model)

- **Puanlar neredeyse aynı** (bölüm 3). Modeller arası fark küçük; asıl fark cihaz (persona) farkı. Bu, bulguların model seçiminden büyük ölçüde bağımsız olduğunu gösterir (aynı model ailesi uyarısıyla).
- **Fable:** En operasyonel ve en çok web doğrulaması yapan model (PC 4, TV 3, mobil 3 arama). Gerçek görünürlük bulguları (AlternativeTo, Softpedia, winget, DonanımHaber) ve satıcı ekosistemi (MAC aktivasyonu) içgörüsü Fable'dan.
- **Opus:** En stratejik ve risk odaklı. Tizen için eşlik uygulaması, Xtream sağlık paneli, imzalı ve denetlenebilir gizlilik paketi, "Sağlayıcı karnesi" ve kota bekçisi fikirleri.
- **Sonnet:** Kısa, kullanıcıya yakın, düşük teknik seviyeyi iyi yansıttı; web araması yapmadı, bu yüzden keşfedilebilirliği tahminle düşük puanladı (PC'de 3; Fable gerçek listelemeleri bulunca 5 verdi).
- **Ders:** Web araması yapan ajanlar gerçek bulgu getirdi; yapmayanlar aynı konuları doğru ama kanıtsız söyledi. Tutarsızlık örneği: Fable TV "hiçbir listede çıkmıyor" dedi, Fable PC 5 kanalda buldu. Fark sorgulardan geliyor (TV: genel "en iyi IPTV" listeleri, PC: "Windows + TiviMate alternatifi"). Birleşik sonuç: **PC kanallarında görünür, TV/satıcı kanallarında neredeyse görünmez.**

## 11. Sonraki adım

1. Bölüm 9'daki soruları yanıtlayın (veya site içeriğini paylaşın), eksik listesini kesinleştirelim.
2. Gerçek veri: Google Search Console, Bing Webmaster, Play Console/Microsoft Store arama terimi raporları, Google Trends (TR, DE, UK, BR).
3. 10-15 kullanıcıyla görüşme veya anket: marka adı, kurulum akışı, fiyat/deneme tercihi.
4. P0 maddeleri (fiyat netliği, güven paketi, marka alt başlığı) düşük maliyetle hemen yapılabilir.
5. İsterseniz aynı deneyi Tizen/webOS ve iOS personalarıyla genişletebilirim.

## Ek: kaynaklar

Rakip analizi ve persona ajanlarının tam kaynak listeleri ilgili raporlarda; başlıca bağlantılar:
- Nightmare TV: AlternativeTo (alternativeto.net/software/nightmare-tv), Softpedia, wingetly, DonanımHaber başlığı
- Windows'ta TiviMate boşluğu: feddit.it/post/3147867, iptvblog.it.com
- Kodi/IPTVnator EPG sorunları: forum.kodi.tv, github.com/4gray/iptvnator
- Mağaza kaldırmaları: storyboard18.com (JioStar 36 uygulama), TorrentFreak (Smarters/Perfect Player/LaLiga; yalnızca arama özeti), AFTVnews (Amazon, yalnızca arama özeti)
- Fiyatlar: slickdeals.net (TiviMate), App Store (IBO, GSE), TroyPoint (OTT Navigator/Televizo; eski olabilir)
