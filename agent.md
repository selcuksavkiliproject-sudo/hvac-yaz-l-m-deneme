# Temsanair AHU hesaplama — Çalışma Hafızası ve Devam Kaydı

**Belge sürümü:** R002  
**Tarih:** 1 Ekim 2026, Europe/Istanbul  
**Güncel uygulama:** R12 / 0.12.0  
**Hesap motoru:** 0.4.1; birim katmanı 1.0.0  
**Durum:** Kullanıcı onayından sonra R12 ana uygulamaya yayımlandı. Kendi sunucusuna kurulacak kimlik/yetki paketi hazır; gerçek DNS/TLS/SMTP ve konteyner kabulü henüz yapılmadı.

Bu bölüm güncel durumdur. Aşağıdaki R001 metni, özgün baytları korunarak tarihsel kayıt olarak eklenmiştir. R001'de geçen R6, eski dosyalar ve o tarihteki açık işler güncel yayın bilgisi sayılmaz. Belge erişilebilen sohbetlerin karar/talep kaydıdır; görünmeyen sohbetlerin kelimesi kelimesine dökümü olduğu iddia edilmez.

## R002.1 — Onay ve sürümleme

Kullanıcının son talimatı: **“Onaylıyorum işleme devam et”** (01.10.2026, 16:09 Türkiye saati). R7–R12 boyunca ana uygulamayı ve özgün agent.md'yi değiştirmeden önce demo onayı bekleme koşulu bu onayla kalktı. Onaylanan demo ana uygulamaya aktarıldı; yeni çalışma hafızası R002 oluşturuldu.

- Özgün R001 dosyası değiştirilmedi: `agent_versions/agent_R001_2026-09-29.md`.
- R001 SHA-256: `1e149d4fb388ef4c951a9a66d25a99d5ebe0bbd445a7342705ac8ff2bb5ab54b`.
- Güncel `agent.md` ve `agent_versions/agent_R002_2026-10-01.md` bayt olarak aynıdır.
- Bundan sonraki yeni çalışma R003 olarak kaydedilir; R001/R002 snapshot'larının üzerine yazılmaz. Güncel dosyanın kimliği ve sürüm geçmişi korunur.
- Uygulama R12, yazılım paketi 0.12.0, yayın sisteminin sürüm numarası 5, bu belge R002 ve kullanıcının cihaz projesinin R numarası farklı kavramlardır.

## R002.2 — Ana uygulama ve yayın kanıtı

**Ana uygulama:** https://temsan-ahu-global.selcuksavkili-projec.chatgpt.site

| Alan | Doğrulanan değer |
|---|---|
| Uygulama adı | Temsanair AHU hesaplama |
| Ana proje kimliği | appgprj_6abacfa82e908191abc4c71f016ddc8e |
| Onay öncesi ana kaynak | 45da545b9067862b0bf5cf66a70eafeb3af14dd8 |
| Onaylanan demo kaynağı | 054bcd3980e76cb91a606e8c90bfb4ebc0b63d88 |
| Yayımlanan ana kaynak | 1c9b3ce43f909fd1b1b1618bf60f028d3d1c6385 |
| Yayın sürümü kimliği | appgprj_6abacfa82e908191abc4c71f016ddc8e~appgver_4dc31be3b2b48191a1f73c79d1e8ed4b |
| Dağıtım kimliği | appgdep_6abe5dba936c8191b0ab49bbe755be0a |
| Sonuç | succeeded |
| Başarı zamanı | 2026-10-01 13:19:16 UTC / 16:19:16 Türkiye |
| Erişim | Mevcut özel, sahibine açık erişim korundu |
| Ana kaynak çalışma yolu | /workspace/scratch/d5510f3e0620/temsanair-ahu-main |

Ana kaynak güncel depodan açıldı; eski `ahu-command` R2 ağacı üzerinden geliştirme yapılmadı. Demo kaynak aktarımında ana `.openai/hosting.json` korundu. Ana D1 iklim veritabanı şeması/migrasyonu değişmedi. `src/projectArchive.js` ve `temsan.ahu.archive.v1` anahtarı korundu; mevcut tarayıcı kayıtları için yeni bir zorunlu geçiş yapılmadı. Yayın sonunda kaynak deposu temizdi.

Onay demosu ayrı adresinde korundu: https://temsan-ahu-kontrol-demo.selcuksavkili-projec.chatgpt.site . Sonraki kullanıcı çalışmasında ana adres esas alınır.

## R002.3 — R7–R12 talep ve karar geçmişi

| Aşama | Talep / karar ve sonuç |
|---|---|
| R7 | “Egzoz / rahatlama fanı” → “Egzoz Fanı”; “Üfleme fanı / fan dizisi” → “Üfleme Fanı”; “Ana ısıtma serpantini” → “Isıtma Serpantini”. Ana başlıklar büyük/kalın, alt başlıklar kelime başı büyük. Modül bazlı üretici aksesuarları ve otomasyon simülasyonu hazırlandı. |
| R8 | Tek/çift kat ve dört giriş–çıkış yönü istenmişti; referans görsellerle alternatifler hazırlandı. Kullanıcı bu yön görsellerini beğenmedi ve geri çekti. Bu sürüm güncel görsel kararı değildir. |
| R9 | Kullanıcı yalnız tek kat/çift kat referans görünümü istedi; sabit dört yön seçeneği kaldırıldı. |
| R10 | Sabit açıklamalar yerine seçili modülün adı/açıklaması; her etkin modülün kendi görseli; kullanıcının belirlediği sıraya göre yerleşim istendi ve eklendi. |
| R11 | Ayrık küpler reddedildi. Modüllerin sırayla gelip ortak kasada birleşmesi, modül sırasını değiştirme, çift katta herhangi bir fiziksel modülü üst kata taşıma ve her iki katta hareketli kalın oklar istendi. Kullanıcı ayrıca manuel hava yolu belirlemeyi açıkça yeniden istedi. Bu son talimat, önceki yön seçeneği istememe kararını manuel akış için değiştirdi. |
| R12 | Uygulama adı Temsanair AHU hesaplama; ülkeye göre ilk harften şehir önerileri; manuel aksesuar ekleme; web sunucusu planı; giriş/kayıt/parola yenileme, e-posta doğrulama ve kullanıcı/admin yetkileri istendi. |
| R12 ana yayın | “Kullanım limitleri sıfırlandı, çalışmana devam et” ardından onay demosu tamamlandı. Son açık onayla ana uygulama yayımlandı ve bu R002 kaydı oluşturuldu. |

Kullanıcı düzeltmeleri, eski istekleri yorumlarken esas alınır. Özellikle özgün R001'deki dört sabit yerleşim seçeneği güncel görsel arayüzün tanımı değildir. Güncel seçim tek/çift kattır; modül sırası, katı ve manuel akış ayrı ayarlanır.

## R002.4 — Güncel davranışlar ve sınırlar

### Birleşen 3D/GIF

- Etkin fiziksel modüller ortak kasa/şase üzerinde birleşerek görünür; seçili olmayan hücrelerden hava geçirilmez. Yardımcı aksesuarlar seri hava işleme hücresi gibi çizilmez.
- Seçilen modülün adı, varyantı ve açıklaması üstte değişir; etiketler görüntüye gömülü sabit yazı değildir.
- Görsel sıra sürükleme/sıra düğmeleriyle düzenlenir. Çift katta fiziksel modüller alt veya üst kata atanabilir.
- Katlar bağımsız yönlendirilebilir veya kullanıcının seçtiği sağ/sol kat bağlantısı ve başlangıç katıyla tutarlı bir dönüş yolu gösterilebilir. Kalın hareketli oklar montajdan sonra başlar.
- Modül/varyant/sıra/kat/akış değişince önceki GIF geçersizleşir. Dışa aktarma sırasında değişiklik veya iptal, eski GIF'in indirilmesine yol açmaz. Görsel ayarlar proje JSON ve revizyonlarında saklanır.
- Bu görünüm referanslara dayanan temsilî 3D montajdır; ölçülü imalat CAD'i değildir. Manuel görsel sıralama ve hava yolu, hesap motorunun sabit psikrometrik işlem sırasını veya basınç kayıplarını yeniden çözmez. Termodinamik doğrulama/CFD yapıldığı iddia edilmez.

### Kontrol ve aksesuarlar

- Entalpiye bağlı ekonomizer yararı ile soğutma serpantini çalışma izni ayrıdır. Uygun serbest soğutma önceliklidir; kalan yük için ayarlı gecikmeden sonra serpantin devreye alınabilir. Nem alma isteğinin ayrı davranışı vardır.
- Fan/damper/hava kanıtı, donma ve sensör koşulları; açma/kapama farkı, gecikme ve emniyet kilitlemeleri simülasyonda görünür. Canlı tesise/BMS'ye komut gönderilmez.
- Başlangıç eşikleri “Demo Varsayımı” olarak işaretlenir. Ana yayın onayı, bunları üretici sınırı veya standart zorunluluğu haline getirmez. Projeye göre mühendis/üretici onayı gerekir.
- Systemair, Swegon, Daikin, FläktGroup ve Condair kaynaklarıyla modül bazında basınç şalteri/manometre, servis aydınlatması, gözetleme camı ve ilgili donanımlar araştırıldı. Kaynak/koşul/I/O önerileri uygulamadaki katalog ve kontrol föyünde bulunur. Her aksesuar her cihazda zorunlu kabul edilmez.
- Kullanıcı manuel aksesuarın adını, ilişkili modülünü, pozitif miktarını, birimini ve açıklamasını ekler/düzenler/siler. Veriler `controlDemo.manualAccessories` içinde proje revizyonuyla saklanır ve kontrol raporuna girer. Adet/metraj üretici seçimi yerine geçirilmez.

### Şehir ve eski işlerle uyumluluk

- Seçilen ülke içinde şehir adı ilk harften önerilir; tam ad veya arama düğmesi beklenmez. Türkçe karakter normalizasyonu, klavye seçimi ve eski yanıtın yeni sorguyu ezmesini önleme vardır.
- İklim veri kaynağı, saha yüksekliği/basıncı ve hesap girdilerinin önceki izlenebilirlik kuralları korunur. Şehir eşleşmesi tek başına doğrulanmış tasarım iklimi değildir.
- SI iç hesaplar, SI/IP/girdi birimleri, TR/EN raporlar, JSON aktarımı ve arşiv kimliği korunur. R6 taşınabilir HTML geçmiş teslimdir; bu çalışmada yeni R12 tek dosyalı çevrimdışı sürüm veya Windows EXE üretildiği iddia edilmez.

### Giriş, roller ve kendi sunucusuna kurulum

Sites yayınının mevcut özel erişimi devam eder. “Hesap Ve Yetkiler” içindeki ayrı üyelik ekranı **Giriş Önizlemesi** olarak açıkça etiketlidir; bu yayında aktivasyon e-postası gönderilmez ve uygulamaya ait yeni kullanıcı hesabı açılmaz.

Ayrı web sunucu paketinde Node/Express uygulaması, Keycloak OIDC Authorization Code + PKCE, PostgreSQL ve Caddy HTTPS yapılandırması bulunur. Doğrulanmış e-posta olmadan uygulama oturumu açılmaz. Oturum çerezi Secure/HttpOnly/SameSite; tokenlar sunucuda şifreli tutulur. Durum değiştiren işlemlerde CSRF/Origin denetimi, her istekte rol/hesap kontrolü vardır. Oturum süreleri 30 dakika boşta kalma / 8 saat mutlak süre taslağıdır.

| Rol | Sunucu kayıtları üzerindeki yetki |
|---|---|
| Yönetici | Tüm projeler, roller, hesap durumu ve proje görüntüleme atamaları |
| Mühendis | Kendi projelerini oluşturma/güncelleme; kendisine açılan diğer projeleri okuma |
| Görüntüleyici | Atanmış projeleri okuma/indirme; sunucu kayıtlarını değiştiremez |

Yeni doğrulanmış kullanıcı Görüntüleyici olur. İlk admin doğrulanmış kullanıcının sabit `sub` kimliğiyle sunucu sorumlusu tarafından açıkça atanır; ilk kayıt olana veya e-posta alan adına otomatik admin verilmez. Rol/yetki istemcideki görünür düğmelere bırakılmaz. Tarayıcı çalışma kopyası ile sunucu kaydı ayrıdır; eşzamanlı güncelleme çatışması 409 ile reddedilir.

Gerçek sunucu, iki alan adı, TLS ve SMTP bilgileri bu çalışmaya sağlanmadı. Bu nedenle Docker/Keycloak'ın gerçek ortamda ayağa kalktığı, gerçek e-posta teslimatı ve gerçek PostgreSQL eşzamanlılık/kilit davranışı doğrulandığı söylenmez. Parolalar sohbette istenmez; `deploy/.env` sunucuda yapılandırılır. Sites D1 ve tarayıcı arşivleri PostgreSQL'e otomatik taşınmaz; proje aktarımı JSON/UI ile yapılır.

## R002.5 — Ana sürüm üzerinde doğrulama

| Kontrol grubu | Geçen |
|---|---:|
| Hesap, birim, rapor ve arşiv çekirdeği — r6-core | 139 |
| Otomasyon/kontrol mantığı — r7-controls | 64 |
| Modül sırası, kat, görsel/GIF ve iptal akışları — r11-ui | 51 |
| Şehir, manuel aksesuar ve hesap ekranları — r12-ui | 19 |
| Sunucu kimlik/yetki güvenliği — r12-server | 43 |
| Kurulum yapılandırması — r12-config | 16 |
| Sites worker/yayın paketi | 4 |
| **Toplam ayrı kontrol** | **336** |

Üretim derlemesi başarılıdır. Bazı testler tekrar çalışmıştır; toplamda aynı kontrol bir kez sayılmıştır. R11'in ilk çalışmasında 51 davranış doğrulandıktan sonra çıktı klasörü olmadığı için resim kaydı hata verdi. Test, klasörü oluşturacak ve GIF'i çalışma alanına bağımlı olmayan göreli yola yazacak biçimde düzeltildi; tam tekrar 51/51 geçti.

Arayüz testleri gerçek React etkileşimlerini JSDOM ve Canvas ile çalıştırır; bütün tarayıcıların görsel testinin yerine geçmez. Sunucu testleri gerçek OIDC istemcisi/imzalı test tokenları/PKCE kullanır; kimlik sağlayıcısı taklit edilmiş, veritabanı pg-mem'dir. Gerçek PostgreSQL kilit/eşzamanlılık testi yapılmadı.

Ana sürüm önizlemesi tarayıcıda açıldı; R12 adı, dinamik modül açıklaması, çift kat birleşmiş cihaz ve hareketli hava yolu gözlemlendi. Ekran görüntüsünün ortamlar arası aktarımı başarısız olduğu için bu tur yeni tarayıcı görseli dosyası teslim edildiği iddia edilmez. Yayın başarısı doğrudan başarılı dağıtım yanıtından doğrulandı.

R12 demo hazırlığındaki 390 px mobil inceleme ve üretim bağımlılıkları için sıfır bulgulu npm audit, önceki hazırlık kanıtıdır; bu onay turunda tekrar yapılmış sayılmaz. Geliştirme araç zincirindeki drizzle-kit alt bağımlılıklarına ait dört orta seviye kaydın üretim konteynerine kurulmadığı önceki raporda açıklanmıştır. Başarılı test, bağımsız güvenlik sertifikası veya hatasızlık garantisi değildir.

Başlıca değişen dosyalar: `src/App.jsx`, `ConfigurationAnimation.jsx`, `visual/assembly.js`, `visual/dynamic.js`, `CitySearch.jsx`, `ControlDemo.jsx`, `ManualAccessories.jsx`, `AccountPanel.jsx`, `ClimatePanel.jsx`, ilgili CSS; `src/controls/`, `src/data/`, `public/assets/reference-r11/`; `worker/city-match.js`, iklim/session yolları; `server/`, `deploy/`, `themes/`, bağımlılık kilidi ve testler. Ana sürüme aktarımda yayın etiketleri ve rapor adı R12 olarak düzeltildi, `AGENTS.md` onay kaydı eklendi. Veri uyumluluğu için `controlDemo` gibi kayıt anahtarları değiştirilmedi.

## R002.6 — Teslimler ve devam işleri

- `Temsanair_R12_Onayli_Web_Server_Paketi.zip`: Onaylı ana kaynak, sunucu/kimlik teması, kurulum örnekleri ve QA kayıtları. Gerçek sırlar veya node_modules içermez.
- `Temsanair_R12_Onayli_Kurulum_Notlari.md`: Kurulum, kullanıcı rolleri, yedekleme, kabul ve R12 yayın notları.
- `agent.md` ve `agent_R002_2026-10-01.md`: Güncel ve değişmez R002 kopyası.
- Eski demo paketi ve R001 teslimleri tarihsel olarak korunur; onaylı paketin yerine kullanılmaz.

Sunucu paketi: 32950381 bayt, 389 dosya. SHA-256: `9280e76ae9e6a756f0f2352eb937d63c9bbf14d71a9b5262f2a5a64004a81503`. Kurulum notlarının SHA-256 değeri: `51f6194242588dd30309cf43b3c0af304f8f7b64484fbcf95e3d2f015b4c81ec`.

Sonraki çalışma için:

1. Güncel agent.md ve ana sitenin gerçek kaynak/yayın durumunu yeniden doğrula; bu kayıttaki geçici dosya yolunun kalıcılığını varsayma.
2. Kullanıcının kendi sunucusuna kurulum istenirse alan adı ve SMTP yapılandırmasını güvenli sunucu ortamında tamamla. Gerçek kayıt/aktivasyon/parola yenileme, üç rol, hesap iptali, eşzamanlı kayıt, yedekten dönüş ve TLS kabulünü yap. E-posta testi yalnız belirlenmiş yetkili test alıcısına gönderilir.
3. Üretici katalogları, gerçek serpantin/fan eğrileri, geometri, basınç/ses ve mevzuat uygunluğu olmadan kesin ekipman seçimi/imalat onayı verildiğini söyleme.
4. Onay sonrası özellik kapsamı dışındaki yeni geliştirmeleri ayrı çalışma olarak kaydet; mevcut kayıtları silme. Yeni belge sürümü R003 olacaktır.

---

# Tarihsel Ek — R001 özgün metni

Aşağıdaki içerik 29.09.2026 tarihindeki kayıttır. İçindeki “güncel”, “bu tur” ve “sonraki revizyon R002” ifadeleri yalnız o tarihi anlatır. R002 bölümündeki düzeltmeler ve yeni onaylar bugünkü çalışma için üstündür. Özgün R001 dosyası ayrıca değişmeden korunur.

# TEMSAN AHU — Çalışma Hafızası ve Devam Kaydı

**Belge sürümü:** R001  
**Tarih:** 29 Eylül 2026, Europe/Istanbul  
**Proje:** hvac yazılım / TEMSAN AHU Global İklim ve Mühendislik  
**Kullanıcı:** Selçuk Şavkılı  
**Son doğrulanan uygulama:** R6 / 0.6.0  
**Hesap motoru:** 0.4.1 — kullanım raporundaki sürüm  
**Birim katmanı:** 1.0.0 — kullanım raporundaki sürüm  
**Kayıt amacı:** Projenin gereksinimlerini, kararlarını, sohbetlerden erişilebilen talimatlarını, teslimlerini, doğrulama düzeyini ve devam işlerini tek yerde korumak.

## 1. Kapsam ve doğruluk

Bu belge, bu oturuma aktarılan HVAC proje sohbetleri, erişilebilir proje dosyaları, güncel R6 kullanım/test raporu, uygulama paketi ve yayın kayıtları esas alınarak hazırlanmıştır. Sohbet aktarımında “conversation too long” ile atlanmış bölümler vardır. Bu nedenle belge **bütün geçmiş sohbetlerin eksiksiz veya kelimesi kelimesine dışa aktarımı değildir**. Erişilen talepler aşağıda korunmuş; asistanın tekrar eden ilerleme mesajları aşama bazında özetlenmiştir. Görülmeyen mesajlar, testler, çalışmalar ve dosyalar uydurulmaz.

Önceki konuşmadaki iddia ile bu turda doğrulanan durum birbirinden ayrılır. Kaynak dosya veya yayın kanıtı, eski durum özetinden daha güncelse esas alınır. Bu oturumun başında son yayımlanmış sürümün R5 olduğu söylenmişti; dosya ve yayın incelemesi **R6'nın da yayımlanmış olduğunu** ortaya çıkardı. Bu belge o durum bilgisini düzeltir.

## 2. Belge sürümleme kuralı

1. `agent.md`, çalışma hafızasının güncel okunabilir kopyasıdır.
2. İlk özgün kayıt `agent_R001_2026-09-29.md` adıyla aynı içerikte saklanır. Bu tarihli kopya sonraki işlerde değiştirilmez veya üzerine yazılmaz.
3. Sonraki çalışma R002, R003… numarasıyla yeni bir tarihli kopya oluşturur. Numaralar yeniden kullanılmaz; ara çalışmalarda da mevcut son numara kontrol edilir.
4. Her yeni sürüme talep, yapılan değişiklikler, değişen dosyalar, test kanıtları, yayın durumu ve kalan işler eklenir. Önceki kayıtlar silinmez. Yanlış eski bilgi silinerek gizlenmez; düzeltme notuyla açıklanır.
5. Güncel `agent.md` aynı dosya kimliği üzerinden sürüm geçmişi korunarak güncellenir; ayrıca yeni tarihli snapshot ayrı dosya olarak kaydedilir.
6. Yeni sürüm, önceki tarihli snapshot'ın SHA-256 değerini değişiklik kaydında belirtir. Aynı sürümdeki `agent.md` ve tarihli snapshot bayt olarak eşit olmalıdır.
7. Gelecekteki ajan/çalışma, işe başlamadan güncel `agent.md` ile uygulamanın mevcut kaynak ve yayın durumunu okur. Belgedeki eski yolun var olması tek başına güncellik kanıtı değildir.
8. Bu kural çalışma sırasında uygulanacak kayıt düzenidir; kendi kendine çalışan bir zamanlayıcı veya bağımsız arka plan yedekleme hizmeti kurulmuş değildir.

### Birbirinden ayrı sürüm numaraları

| Kavram | Bu kayıttaki değer | Anlamı |
|---|---|---|
| Çalışma hafızası | R001 | Bu `agent.md` belgesinin revizyonu |
| Uygulama sürümü | R6 / 0.6.0 | Kullanıcıya sunulan yazılım sürümü |
| Yayın sisteminin sürümü | 4 | Ana sitenin yayın sistemindeki sıra numarası; uygulama R4 demek değildir |
| Mühendislik proje revizyonu | Projeye göre R1, R2… | Kullanıcının uygulamada kaydettiği belirli cihaz hesabının geçmişi |

## 3. İş hedefi ve kullanıcı tercihleri

TEMSAN için AHU hesap, ön seçim, raporlama ve görsel anlatımı aynı proje verisine bağlayan bir mühendislik uygulaması geliştirilir. Kullanıcı makine/HVAC mühendisi olarak izlenebilir girdiler, açık formüller, kaynaklar, ölçü birimleri ve uygulanabilir çıktılar ister. Arayüz Türkçe karakterleri doğru göstermeli; mesleki kullanıma uygun, anlaşılır ve kolay olmalıdır.

Kalite talebi: hesap, modül seçimi, iklim girdileri, proje saklama, rapor ve animasyon birlikte incelenir; bulunan hatalar giderilir. “Mükemmel sonuç” talebi, kanıtsız kusursuzluk/sertifikasyon iddiasına çevrilmez. Test edilmeyen cihaz, tarayıcı veya senaryo açık belirtilir.

Masaüstü ve telefon kullanımına uygun erişim ile indirilebilir çalışma istenir. Mevcut teslim web uygulaması ve taşınabilir HTML'dir; doğrulanmış bir Windows kurulum paketi, `.exe`, iOS veya Android mağaza uygulaması teslim edildiği iddia edilmez.

## 4. Güncel ana uygulama ve teslimler

**Ana uygulama:** https://temsan-ahu-global.selcuksavkili-projec.chatgpt.site

| Çıktı | Durum ve kullanım |
|---|---|
| `HVAC_AHU_Prototip.html` | Güncel R6 taşınabilir uygulama; 11.748.894 bayt. İndirilip tarayıcıda açılan sürüm |
| `HVAC_AHU_R6_Kullanim_ve_Test_Raporu.md` | Birim, dil, rapor, revizyon, yedekleme ve test sınırlarını açıklayan güncel rapor; 5.613 bayt |
| `TEMSAN_AHU_R6_Gorunumu.jpg` | Mevcut başarılı yayına bağlı R6 ekran görüntüsü; bu turda yeni bir tarayıcı testi yapılmış anlamına gelmez |
| `agent.md` | Güncel çalışma hafızası R001 |
| `agent_R001_2026-09-29.md` | İlk özgün çalışma hafızasının değiştirilmeyecek kopyası |

Güncel HTML ve rapor bu turda kayıtlı dosyalardan yeniden alınmış, çalışma alanındaki aynı adlı çıktılarla bayt düzeyinde eşit bulunmuştur.

### Dosya bütünlüğü

| Dosya | SHA-256 |
|---|---|
| HVAC_AHU_Prototip.html | `2f72054bd3a5e2b32c4d6565efff2e24ed7603b6be0b27e6b990090418cf9f68` |
| HVAC_AHU_R6_Kullanim_ve_Test_Raporu.md | `476c4d4de4aa2fa511b92cd7642d37544eabed67f5b9ebd1c86b400d0bd0d398` |

### Yayın doğrulaması

- Ana site kimliği: `appgprj_6abacfa82e908191abc4c71f016ddc8e`.
- Kayıtlı son yayın sürümü: 4.
- Kaynak commit: `45da545b9067862b0bf5cf66a70eafeb3af14dd8`.
- Yayın durumu: `succeeded`.
- Yayın durumunun güncellenmesi: 29.09.2026 18:05:58 UTC / 21:05:58 Türkiye saati.
- Yayına bağlı görüntüde R6 etiketi, sunum birimleri, “Birimleri değiştir”, “Projeler / yeni çalışma / revizyonlar” ve dört yerleşim seçeneği görülmüştür.
- Bu oturumda uygulama kodu değiştirilmemiş ve yeniden yayın yapılmamıştır; var olan son çıktı doğrulanıp sunulmaktadır.
- Yerel R6 dağıtım arşivi ile sunucudaki arşivin bire bir bayt eşitliği bu turda doğrulanmamıştır. Yayın başarısı, bütün kullanıcı akışlarının gerçek tarayıcıda geçtiği anlamına gelmez.

## 5. Temel gereksinimler ve kabul edilen davranışlar

### 5.1 Hesap ve kaynak izlenebilirliği

- Hesap motorunun iç birimleri SI olarak kalır.
- Girdiler proje/cihaz kimliği, kaynak ve gerekirse varsayım açıklaması ile ilişkilendirilir.
- Isıtma, soğutma, nem alma/verme, filtreler, ısı geri kazanımı, fanlar ve desteklenen diğer AHU modülleri yalnız etkin konfigürasyona göre değerlendirilir.
- Sonuç değişikliği gerektiren girdi değiştiğinde eski sonuç, rapor ve GIF geçerliymiş gibi kullanılmaz.
- Çözülmeyen özel modül için performans veya kapasite uydurulmaz.
- Üretici fan/serpantin eğrileri ve doğrulanmış katalog verisi olmadan hesap sonucu kesin ürün seçimi veya sertifikalı performans olarak sunulmaz.

### 5.2 Konum ve çevrimiçi iklim

- Akış: ülke → şehir → yakın istasyon → kaynaklı iklim koşulu → saha yükseltisi/basınç → AHU hesabı.
- Proje sahası ülkesi/konumu ile veri istasyonu ülkesi/konumu ayrı tutulur.
- Saha yükseltisi ile meteoroloji istasyonu yükseltisi aynı kabul edilmez.
- Dönem, istasyon, kaynak, tasarım yüzdeliği, veri yeterliliği ve kullanılan yöntem kayıtlı olmalıdır.
- Önceki R3 teslim kaydında 34.146 yerleşim ve 17.313 istasyon bildirilmiştir. Bu sayılar bu turda yeniden sayılmamıştır.
- Önceki akış NOAA arşivinden talebe bağlı veri alma ve saklamayı destekler. Açık arşivden hesaplanan koşul, resmî ASHRAE tasarım tablosu diye etiketlenmez.
- Lisanslı ASHRAE verileri için yetkili veri/kaynakla içe aktarma yolu bulunur; çevrimiçi bağlanmak lisans koşullarını kaldırmaz.
- Mutlak sıcaklık rekorları HVAC tasarım koşulları yerine geçirilmez. Farklı zamanların sıcaklık/nem uçları tek fiziksel hava noktası gibi birleştirilmez.
- Kahramanmaraş için önceki incelemede yeterlilik eşiğini sağlayan 9 yıl bulunduğu ve belirlenmiş 10 yıllık ön tasarım kapısının geçilemediği bildirilmiştir. Bu, projenin tanımlanmış veri kapısıdır; evrensel standart şartı olarak ileri sürülmez. Yeni veri gelmeden kilidin kendiliğinden kalktığı varsayılmaz.

### 5.3 Konfigürasyona bağlı hareketli cihaz anlatımı

Görsel, seçilen ve hesaplanan gerçek konfigürasyondan kurulmalıdır. Örneğin ısı geri kazanımı kapalıysa cihazda geri kazanım hücresi ve ona ait hava yolu/etiket bulunmaz. Dönüş filtresi ve egzoz fanı kendi seçimlerine bağlıdır.

| Yerleşim | Hava yolu ve ağızlar |
|---|---|
| Tek kat düz | Giriş ve çıkış karşı cephelerde |
| Çift kat karşı akış | Alt üfleme ve üst egzoz yolları |
| Tek kat U dönüş | Aynı cephede, aynı kotta giriş/çıkış; yan yana iki sıra |
| Çift kat U dönüş | Aynı cephede alt giriş/üst çıkış |

- Sağ/sol giriş yönü ve desteklenen U dönüş konumu seçilebilir.
- Modül kaldırılınca hava yolu ve kalan hücrelerin sırası yeniden kurulur.
- U dönüş basınç kaybı fan hesabı, animasyon ve raporda aynı veriden okunur.
- U dönüş kaybı bilinmiyorsa boş değer “bilinen 0 Pa”ya çevrilmez; fan sonucu ön değerlendirme olarak işaretlenir. Kaynağı yön değişimiyle kaybolmaz.
- Hava ışıklı izlerle hareket eder; geçilen modül vurgulanır ve hesap kartı güncellenir.
- Filtrede Pa; serpantinlerde kapasite ve sıcaklık değişimi; nemlendiricide kg/h; fanda debi, basınç ve güç görünür.
- Fan dönüşü, soğutmada yoğuşma ve nemlendirmede buhar hareketi görsel anlatımdır.
- Kullanıcı panelleri/kesiti, bakış açısını, odağı ve animasyon duraklatmayı kontrol edebilir; destek kapsamı kullanılan sürüme bağlıdır.
- Kullanıcının onayladığı görünüm gerçekçi metal/doku ve iç ekipman anlatımıdır. Mevcut görsel 2.5D konsepttir; CFD, ölçülü imalat CAD'i veya BMS canlı ölçümü değildir.

### 5.4 GIF çıktısı

- GIF, o an hesaplanan cihazın etkin modülleri ve güncel verileri üzerinden oluşturulur.
- Dosya indirildiğinde uygulama açık olmadan hareketli biçimde izlenebilir.
- Modül/girdi değişince önceki GIF geçersizleşir; yeniden üretim gerekir.
- Her hücre sırasıyla vurgulanır; kapasite/basınç ve hava koşulları aynı hesap kaydına bağlıdır.
- Önceki gerçekçi R1 taslakta 1280 × 900, 14,4 saniye, 144 kare ve yaklaşık 4,5 MB bildirilmiştir. Bu ölçüler bütün sonraki GIF'lerin sabit özelliği değildir.
- Master R2 ve R5 için dört yerleşim GIF'inin bağımsız okuyucuyla doğrulandığı önceki teslim kayıtlarında bildirilmiştir.

### 5.5 Giriş ve sunum birimleri

- Ayarlardan SI, I-P veya özel sunum seçimi yapılır.
- Sayısal değer girilirken o girdinin birimi ayrıca seçilir.
- Sonuçların hangi birim sisteminde gösterildiği arayüzde görünür.
- Orijinal değer/birim, dönüşüm katsayısı/ofseti ve SI karşılığı izlenir.
- Mutlak sıcaklık ile sıcaklık farkı ayrı büyüklüklerdir: °F dönüşümünde ofset, Δ°F dönüşümünde yalnız ölçek vardır.
- Boyutsal olarak uyumsuz birimler reddedilir.
- Birim seçimi fiziksel sonucu değiştirmez; yalnız giriş/gösterim temsili değişir.
- Rapor, modül, iklim gösterimi ve GIF proje sunum tercihini kullanır.
- Btu türü International Table, gallon US liquid olarak raporda tanımlıdır. Nem oranı kuru hava esaslıdır; entalpi dönüşümü referans sıfırını değiştirmez.

### 5.6 Kısa ve ayrıntılı rapor

| Rapor | İçerik |
|---|---|
| Kısa | Genel sistem sonuçları, modül bilgisi, gereksinimler ve eksikler |
| Ayrıntılı | Cihaz koduna bağlı etkin modül föyleri, çalıştırılan formüller, sayısal yerine koymalar, girdi/kaynak izleri ve denge kontrolleri |

- Formül yerine koymaları ve kabul toleransları SI olarak açıkça etiketlenir; sonuçlar seçilen sunum birimindedir.
- Egzoz fanı, nemlendirici besleme suyu ve modül kesit hesaplarının sayısal izleri kapsamda yer alır.
- HTML indirme ve tarayıcı üzerinden Yazdır/PDF akışı vardır.
- Her proje kaydı bir AHU cihaz kodunu temsil eder; birden fazla cihaz için ayrı çalışma açılır. Tek kayıtta doğrulanmış çok cihazlı tesis yönetimi varmış gibi anlatılmaz.

### 5.7 Proje ve revizyon geçmişi

- Eski revizyon özgün haliyle kalır; düzenleme yeni revizyon üretir.
- Eski kayıt açılabilir; “Yeni revizyon olarak geri yükle” önceki girdileri en yüksek numaranın sonrasına taşır.
- Açıklamalı revizyon kaydı desteklenir.
- Referanstan yeni proje yeni kimlik ve R1 ile açılır. Modül/girdi/birim/dil tercihleri kopyalanır; kaynak proje değişmez.
- Yeni işte konum, iklim, yük ve kaynak geçerliliği yeniden incelenir; referans sonuçları otomatik doğrulanmış kabul edilmez.
- Proje JSON kaydı revizyonları içerir; tüm arşiv ayrıca yedeklenebilir.
- Arşiv birleştirmesinde çakışma sessizce üzerine yazılmaz. Dış dosyadan gelen sonuç yeniden hesaplanır.
- Arşiv şu anda cihazın tarayıcısındadır; bulut/cihazlar arası senkronizasyon yoktur. Tarayıcı verisi silinirse JSON yedeği gerekir.
- R6 öncesinde hiç kaydedilmemiş revizyonlar sonradan üretilemez.

### 5.8 Dil

- Türkçe ve İngilizce arayüz, rapor ve animasyon metinleri desteklenir.
- Proje adı, müşteri notu ve özgün kaynak metni çevrilerek değiştirilmez.
- Dil tercihi projeyle saklanır.
- Dil paketi JSON şablonu indirme/yükleme yolu vardır; eksik/geçersiz paket reddedilir. Yeni dilin teknik doğruluğu insan incelemesi gerektirir.

## 6. Sohbet ve çalışma kronolojisi

| Aşama | Erişilebilir konuşmadaki gelişme | Kanıt düzeyi |
|---|---|---|
| Başlangıç / R0–R2 | HVAC ajanı, veri formu, hesap/ekipman akışı ve profesyonel uygulama hedefi; modüler AHU arayüzü | Önceki bağlam, R0/R2 yerel çıktıları |
| R3 | Çevrimiçi ülke/şehir/istasyon/iklim akışı; basınç ve saha yükseltisi; NOAA ve yetkili veri ayrımı | Önceki teslimde 895 kontrol ve 7 arayüz senaryosu bildirilmiş |
| İlk 3B demo | Modül hesapları, yaz/kış, temiz/kirli filtre, döndürme ve kesit; ana uygulamadan ayrı onay aşaması | Önceki teslimde 138 eşleme kontrolü bildirilmiş |
| Gelişmiş akış | Işıklı hava izleri, sinematik görünüm, proje yükleme, akışı takip et, otomatik modül kartı | Aktarılan sohbet kayıtları |
| Gerçekçi GIF R1 | Kullanıcının iki görseline göre metal gövdeli kesit ve hareketli GIF taslağı | R1 GIF/HTML çıktıları mevcut; bu tur yeniden oynatım testi yok |
| Master R2 | Dört yerleşim, giriş yönü, U dönüş, seçilmeyen modülün kalkması | Önceki teslimde 50 hesap/yerleşim ve 16 olay testi; gerçek tarayıcı sınırı |
| R5 entegrasyonu | Kullanıcının açık onayıyla ana uygulamaya entegrasyon; U kaybı, fan, rapor ve GIF tutarlılığı | Önceki teslimde 990 kontrol ve dört GIF doğrulaması bildirilmiş |
| R6 | Birim, dil, kısa/ayrıntılı rapor, revizyon, referans proje ve yedekleme | Güncel kayıtlı rapor, HTML, dağıtım paketi ve R6 yayın görüntüsü |
| Bu kayıt / R001 | `agent.md`, özgün kopya ve son çıktının sunulması | Dosya/yayın incelemesi ve bu teslim |

Sayısal örnekler olan 59,52 kW kış ısıtma veya 7,24 → 5,98 kW fan değişimi eski demo senaryosuna aittir; bütün projelere uygulanacak sabit tasarım değeri değildir.

## 7. Kullanıcı talepleri ve onay kaydı

Aşağıdaki alıntılar erişilebilir proje sohbetinden alınmıştır; yazım kullanıcıdaki haliyle korunmuştur. Aradaki asistan mesajları bu belgenin kronoloji ve gereksinim bölümlerinde özetlenmiştir.

### Çevrimiçi iklim talebi

> Çalışmana ek olarak Verileri toplu çekmek lisans gerektiriyorsa çevrimiçi bilgileri çekilebileceği bir bağlantı yap tasarım yapılacak şehir ülke girildiğinde çevrimiçi bu verileri alabileceğin kullanabileceğin bir uygulama olarak oluştur

### İlk animasyon ve onaylı demo talebi

> Hesaplanan ve seçilen çihazın 3d hava akılı similasyon ve hava akılı sırasında cihazın modülündeki işlemi örneğin filtrele için hesap edilen veri akışta veril bilgisi olarak görünsün ısıtmadan geçerken ısıtma miktarı görünsün bunu önce demosunu oluştur onayımdan sonra uygula

> Bu veriler seçilen hesaplanan çihazda animasyon şeklinde hava akışı ve verilerin olmasını istiyorum görsel şölen yap bana

> Görselin hareketli animasyon şeklinde olmasını istiyorum hava hareket edecek ve geçtiği her hücre verisi görünecek canlı akış gibi düşün bunun için ne yapabilirsin

### Konfigürasyon ve GIF

> Animasyonu seçimi yapılan cihazdaki konfigürasyona göre ayarla ve hazırla örneğin ısı geri kazanım olman cihaz hesaplaması yapılıyorsa görselden o modülü kaldır gösterme. Bu bilgilere göre hareket animasyonu ayarla ve yazılama ve uygulamada çalıştıracak şekilde master çalışmanı bana sun

> Bunlara ek olarak Animasyonu gif olarak oluştur ve indirilebilir olsun. İndirildiğinde hareketli animasyonu izleyebileyim

> Gift animasyonda kullanacağım görsellerdeki gerçeğe yakın görümü bu şekilde görsel istiyorum. Bu şekilde gerçekçi bir tasarım üzerinden hareketli animasyon gift taslağı oluştur onayımdan sonra final uyumayı hazırla

Bu talebin yanında iki görsel bulunduğu aktarılan konuşmada görülüyor. Özgün iki görselin kimlikleri bu kayıt kapsamında kesin eşleştirilmemiştir; başka resimler bunların yerine varsayılmaz.

> Ünitenin tek veya çift katlı olması seçilebilir olsun seçimde olması gereken modüller örneğin sogutma ısıtma filtreleme gibi hangi modül hesabı seçimi yapılmışsa ünite tasarımında tek kat çift kat hava ve hemde hava akışına göre bir taraf giriş diğer tara çıkış veya modül dizilimi u çekerek giriş ve çıkış tek katta aynı yönde gibi alternatif tasarılarıda kapsayacak gift olarak hareketli animasyonu tekrar kurgula ve bu senin master çalışman olacak şekilde çıktı ver . Çıktı incelememde onay alırsan bunu uygulamaya ekle

### Ana uygulamaya entegrasyon onayı

> Ana uygulama ekle uygulamanın her noktasını incele test et eksikleri gider bana mükemmel sonucu verene kadar bu işlemi tekrarla

Bu mesaj, Master R2'nin ana uygulamaya eklenmesine ilişkin açık onaydır. Önceki “demo onayından sonra ekle” beklemesi bu onayla aşılmıştır. Aynı kapsam için yeniden onay istenmez.

### R6 işlev talebi

> Hesaplama verilerin ayarlar kısmından birim seçimi örneğin m yerine inç gibi tüm hesaplamalarda kullanılacak birim çeşidini seçme , değer girilirken girilen birim türü seçimi ve girilen verilerin tamamının hangi birim sisteminde sunulacağı gösterilsin. Hesaplama sonrası detaylı rapor tüm hesaplama formülleri ile her ünite için oluşturulsun kısa raporda hesap sonuçları ve modül bilgisi ile genel sistem raporu olsun. Revizyon numarası ve çalışmanın önceki sürümlerine ulaşılabilir olsun. Yeni bir çalışmaya başlarken daha önce yapılan çalışmalardan referansla başlayabilecek yapının olmasını istiyorum. Eski projeyi getirip değişmesi gereken verilerileri girerek hızlı yeni proje çalışma oluşturulsun

Aktarılan asistan çalışma kayıtlarında Türkçe/İngilizce ve ek dil paketi de bu geliştirmeye eklenmiştir. Bu eklemenin ayrı kullanıcı mesajı aktarılan kesitte görülmediğinden böyle bir mesaj uydurulmaz.

### Çalışma hafızası ve son çıktı talebi

> Yapılan çalışmaların ve sohbetlerin tamamını agent.md dosyası oluştur kaydet. Her yeni çalışma için bu dosyanın özgün halini koru versiyon atayarak kaydetmeye devam et

> çalışmanın ilerlemesinde sorun mu var şuan ne yapıyorsun

> agent.md oluşturduktan sonra çalışmanın son çıktısını göster

## 8. Test kanıtları ve sınırları

Güncel R6 kullanım/test raporu aşağıdaki sonuçları bildirir. **Bu turda 1.145 test yeniden çalıştırılmamıştır.** Sayılar önceki R6 raporundan aktarılır; bu oturumda mevcut dosyalar ve yayın durumu incelenmiştir.

| R6 raporundaki test grubu | Geçen / toplam |
|---|---:|
| Sayısal / iklim denetimi | 674 / 674 |
| Modüler hesap motoru | 116 / 116 |
| Eski motor regresyonu | 87 / 87 |
| Yerleşim entegrasyonu | 66 / 66 |
| Önceki ana arayüz olayları | 27 / 27 |
| Yeni birim / rapor / revizyon / dil çekirdeği | 137 / 137 |
| Yeni arayüz akışları | 34 / 34 |
| Worker / dağıtım paketi | 4 / 4 |
| Toplam | 1145 / 1145 |

Raporda belirtilen kapsam: SI/I-P sonuç değişmezliği; °C/°F/Δ°F; girdi izi; TR/EN × SI/I-P × kısa/ayrıntılı sekiz rapor; modül/formül kapsamı; özel isimlerin korunması; JSON yedek/geri alma; kota/bozuk arşiv; eski revizyonun korunması; yeni proje kimliği; dil paketleri; İngilizce GIF kare/döngü kontrolü; taşınabilir HTML gömmeleri.

Rapora göre arayüz olayları React/JSDOM, gerçek Canvas/GIF ve yerel Worker ile sınanmıştır. Gerçek tarayıcı ekran yerleşimi, telefon, Windows `file://`, işletim sistemi indirme/yazdırma ve fiziksel ağ kesilmesi testleri tamamlanmamıştır. Bunlar tamamlanmış gibi anlatılmaz.

Bu oturumda görülen `ahu-command` kaynak ağacı ve evidence dosyaları R2'ye aittir. R6 uygulama kodu taşınabilir HTML ve dağıtım paketinde bulunmaktadır; R6'nın 1.145 kontrolüne ait bütün ham günlükler bu yerel eski ağaçta bulunmamıştır. Sonraki kaynak değişikliği için önce ana sitenin güncel kaynak checkout'u açılmalıdır.

### Bu turda yapılan kontroller

- Güncel R6 raporu kayıtlı dosyasından okundu.
- Güncel HTML ve rapor alındı; boyutları ve SHA-256 değerleri hesaplandı; aynı adlı yerel çıktılarla eşleşti.
- R6 dağıtım paketinde birim, dil, rapor ve proje geçmişi özelliklerine ait uygulama içeriği incelendi.
- R6 dağıtım paketinin hesap/rapor bileşenleri üzerinde 13 dar kontrol çalıştırıldı ve geçti: 104 °F → 40 °C; 18 Δ°F → 10 ΔK; metre → inç; boyutsal uyumsuzluğun reddi; TR/EN × SI/I-P × kısa/ayrıntılı sekiz rapor; değişmiş girdiye ait eski sonuç raporunun reddi. Sekiz raporun sayısal sonuçları aynı kaldı; ayrıntılı raporların her birinde 23 çalıştırılmış hesap kodu bulundu. Bu kontroller gerçek tarayıcı arayüz testi değildir ve geçmiş 1.145 testin yeniden çalıştırılması anlamına gelmez.
- Taşınabilir HTML'de R6 birim/dil/rapor içeriğinin gömülü olduğu ve haricî script/link etiketi bulunmadığı görüldü. Bu bulgu gerçek ağ kesilmesi testinin yerine geçmez.
- Ana site ve son sürüm kaydı okundu; son dağıtımın başarılı durumu doğrulandı.
- Yayına bağlı ekran görüntüsü görsel olarak incelendi; R6 ve yeni ana kontrol bağlantıları görüldü.
- Bu dokümanın özgün snapshot'ı oluşturulurken güncel kopyayla eşitliği kontrol edilir.

## 9. Açık işler ve sonraki çalışma için başlangıç

1. Kaynak değişikliği yapılacaksa ana sitenin güncel kaynak deposunu aç; R2 yerel ağacı üzerinde R6 varmış gibi düzenleme yapma.
2. Gerçek tarayıcıda masaüstü ve mobil akışları tamamla: birim seçimi → hesap → kısa/ayrıntılı rapor → GIF → revizyon → referanstan yeni iş → JSON yedek/geri alma.
3. Gerçek işletim sistemi indirme/PDF yazdırma ve Windows dosyadan açma testlerini yap; çevrimdışı hesap ile çevrimiçi iklim alma davranışlarını ayırarak sınırları belirt.
4. R6 ham test günlüklerini güncel kaynak ağacından bul veya gerekli senaryoları çalıştırıp kanıt dosyalarını sakla. Daha önce raporlanmış sayıyı yeni test sayısı olarak sunma.
5. Üretici verileri gerektiren kesin ekipman seçimi, glikol ve gerçek fan/serpantin eğrilerini kapsam ve veri kaynağı netleşmeden tamamlandı sayma.
6. Yeni iş ve bulgularla `agent.md` R002'yi oluştur; R001 snapshot'ını değiştirme.

## 10. Erişilebilir önceki teslimlerin envanteri

Bu liste proje devamı için yer gösterir; eski çıktılar güncel R6 yerine kullanılmaz. Listede bulunmak, bu turda yeniden test edilmiş olmak anlamına gelmez.

| Dosya / grup | Rol |
|---|---|
| `AHU_R3_Denetim_ve_Kullanim_Raporu.md` | Çevrimiçi iklim katmanı R3 raporu |
| `HVAC_Iklim_Veritabani_R3.sqlite` | Önceki teslimde bağlantısı verilen iklim veri tabanı; bu tur içeriği okunmadı |
| `AHU_3B_Hava_Akisi_Demo.html` | Ayrı ilk hareketli cihaz demosu |
| `AHU_Gercekci_Akis_Taslagi_R1.gif` | Gerçekçi görsel onay taslağı |
| `AHU_Gercekci_GIF_Taslak_R1.html` | R1 oynat/duraklat önizlemesi |
| `AHU_Master_R2.html` | Dört yerleşim için etkileşimli master taslağı |
| `AHU_Master_R2_Tek_Kat_Duz_Akis.gif` | Tek kat düz örnek |
| `AHU_Master_R2_Cift_Kat_Karsi_Akis.gif` | Çift kat karşı akış örnek |
| `AHU_Master_R2_Tek_Kat_U_Donus.gif` | Tek kat U örnek |
| `AHU_Master_R2_Cift_Kat_U_Donus.gif` | Çift kat U örnek |
| `AHU_Master_R2_Tam_Paket.zip` | Master R2 kaynak/örnek/test paketi |
| `HVAC_AHU_R5_Test_ve_Kullanim_Raporu.md` | R5 ana uygulama entegrasyon kaydı |
| `temsan-ahu-r6-site.tar.gz` | Yerelde bulunan R6 dağıtım paketi; güncel kaynak checkout'unun yerine geçmez |

Ayrı demo adresi: https://temsan-ahu-3d-demo.selcuksavkili-projec.chatgpt.site. Güncel mühendislik çalışması için ana uygulama adresi esas alınır.

## 11. R001 değişiklik kaydı

| Alan | Kayıt |
|---|---|
| Talep | Çalışmaları/sohbetleri agent.md ile kaydet; özgünü koruyup sürümle; son çıktıyı göster |
| Yapılan | Erişilebilir bağlamı düzenleme, gereksinim/onay ve sürüm tarihçesini kayıt, R6 dosya/yayın kontrolü, ilk değişmez snapshot |
| Düzeltme | Önceki “son sürüm R5 / R6 doğrulanmadı” durum bilgisi R6 yayın kanıtıyla güncellendi |
| Uygulama değişikliği | Yok; mevcut son sürüm sunuldu |
| Test beyanı | R6 raporunda 1145/1145; bu tur yeniden koşulmadı. Bu tur ayrıca 13 dar hesap/rapor kontrolü geçti; dosya/yayın kontrolleri yapıldı |
| Sonraki belge revizyonu | R002 |
| Özgün kayıt | agent_R001_2026-09-29.md |
