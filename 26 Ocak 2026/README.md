# Kur'ancılar — Birleşik Stratejik, Teknik ve Mali Rapor

**Site:** [https://kuran.yasireymen.com](https://kuran.yasireymen.com)
**Rapor Türü:** Hem İç Ekip Hem Kamuoyu İçin Bütüncül Rapor (Markdown)
**Hazırlayan:** Yasir Eymen Kayabaşı
**Rapor Tarihi:** 26 Ocak 2026
**Zaman Ufku:** 12–24 Ay (Uzun Vadeli)

---

## İçindekiler

1. [Yönetici Özeti (Executive Summary)](#yönetici-özeti-executive-summary)
2. [Amaç, Kapsam ve Hedef Kitle](#amaç-kapsam-ve-hedef-kitle)
3. [Ana Bulgular — Kısa Özet](#ana-bulgular--kısa-özet)
4. [Kullanıcı Davranışı ve Elde Tutma Analizi](#kullanıcı-davranışı-ve-elde-tutma-analizi)
5. [Trafik Kaynakları ve Keşif Fırsatları](#trafik-kaynakları-ve-keşif-fırsatları)
6. [KPI’lar ve 12–24 Ay Hedefleri (GA4 Uyumlu)](#kpilar-ve-12–24-ay-hedefleri-ga4-uyumlu)
7. [GA4 Event Taksonomisi ve Conversion Stratejisi](#ga4-event-taksonomisi-ve-conversion-stratejisi)
8. [Hunî (Funnel) Modeli ve Ölçüm Planı](#hunî-funnel-modeli-ve-ölçüm-planı)
9. [Teknik İnceleme — Mevcut Durum ve Karşılaştırma](#teknik-inceleme--mevcut-durum-ve-karşılaştırma)
10. [Geliştirme Önerileri ve Yol Haritası (Roadmap)](#geliştirme-önerileri-ve-yol-haritası-roadmap)
11. [Mali Analiz ve Sürdürülebilirlik](#mali-analiz-ve-sürdürülebilirlik)
12. [Topluluk, Moderasyon ve İçerik Yönetimi Politikası](#topluluk-moderasyon-ve-içerik-yönetimi-politikası)
13. [Operasyonel ve Güvenlik Önerileri](#operasyonel-ve-güvenlik-önerileri)
14. [Uygulanabilir Eylem Adımları — Hemen Yapılabilecekler](#uygulanabilir-eylem-adımları-—-hemen-yapılabilecekler)
15. [Ekler — Teknik Detaylar ve Referanslar]

---

# Yönetici Özeti (Executive Summary)

Kur'ancılar, "okuma ve düşünme" odaklı, topluluk destekli bir Kur'an platformudur. Bu rapor hem iç ekip hem de geniş kamuoyuna yönelik, platformun analitik düzeni (GA4), teknik altyapı, mali yapı, rekabetçi konum ve 12–24 aylık büyüme stratejisini tek bir Markdown belgesinde birleştirir.

Kısa hedefler:

* Kullanıcı sadakatini (okuma süresi ve tekrar ziyaret) artırmak. 12 ay içinde MAU +%40, 24 ayda +%100 hedefleniyor.
* Derin etkileşimi (seriler, yorum, geri bildirim) ölçülebilir dönüşümlere çevirerek aboneliğe veya sürdürülebilir reklam gelirine bağlamak.
* Teknik olarak modern, erişilebilir ve hızlı bir deneyim sunmak; rakipler (quran.com, kuran.diyanet.gov.tr) ile kıyaslandığında topluluk ve etkileşim avantajı vurgulanacak.

Bu raporun sonunda, hayata geçirilebilir GA4 event taksonomisi, dönüşüm tanımları, öncelikli geliştirme adımları ve finansal sürdürülebilirlik yolu yer almaktadır.

---

# Amaç, Kapsam ve Hedef Kitle

**Amaç:** Kur'ancılar platformunun mevcut dijital-performansını analiz etmek, kullanıcı davranışlarını anlamlandırmak, ölçülebilir KPI’lar belirlemek ve GA4 tabanlı izleme ile topluluk-temelli büyüme stratejisi önermek.

**Kapsam:** GA4 verileri (kullanıcı etkileşimleri, trafik kaynakları, demografi), site performansı gözlemleri, karşılaştırmalı analiz (quran.com, kuran.diyanet.gov.tr), teknik mimari şeması ve maliyet-kârlılık çalışması.

**Hedef Kitle:** İç ekip (ürün, geliştirici, büyüme, moderasyon) ve kamuoyu (kullanıcılar, gönüllüler, potansiyel destekçiler).

---

# Ana Bulgular — Kısa Özet

* Platform **okuma ve düşünme** odaklıdır; kullanıcılar amaçlı geliyor ve oturum süreleri uzun (derin okuma eğilimi).
* Trafiğin büyük kısmı **organik arama** ve **doğrudan erişim**ten geliyor; sosyal trafik zayıf.
* Topluluk etkileşimi (yorum, forum) benzersiz bir değer önerisi sunuyor ama aktif katkı oranı düşük.
* Teknik altyapı modern — PWA, Next.js, Supabase gibi bileşenler kullanılmakta; performans iyileştirmeleriyle mobil deneyim daha da güçlendirilebilir.
* Finansal sürdürülebilirlik için aylık **20.000–25.000 TL** arası gelir gereklidir; bu hibrit modelle (abonelik + reklam) sağlanabilir.

---

# Kullanıcı Davranışı ve Elde Tutma Analizi

## Gözlemler

* Ziyaretçiler amaçlı geliyor: belirli bir sure/ayet aramak, meali okumak veya tartışmaya katılmak.
* Ortalama oturum süresi, derin okuma eğilimini işaret ediyor. Bu nedenle "ortalama oturum süreleri" ticari amaçlı metriklerden daha anlamlıdır.
* İçerik referans niteliğinde — tek seferlik değil, tekrar başvurulan kaynak.

## Riskler

* Tekrar ziyaret oranı (retention) orta seviyede; hatırlatma ve tetikleyici (reminder) mekanizmaları eksik.
* Aktif katkı (feedback_submit, content_suggestion) düşük; düşük bariyerli katkı yolları gereklidir.

## Fırsatlar

* Okuma serileri, hatırlatmalar (push), ve kişiselleştirilmiş okuma geçmişi sadakati ciddi oranda artırabilir.
* Erişim hızına yatırım (resim optimizasyonu, SSR/SSG ayarları) mobil kullanıcı memnuniyetini yükseltir.

---

# Trafik Kaynakları ve Keşif Fırsatları

## Mevcut Dağılım (Nitel)

* Organik Arama: Yüksek — içerik doğru anahtar kelimelerle eşlenmiş.
* Doğrudan: Yüksek — sadık çekirdek kitle.
* Sosyal: Düşük — büyüme alanı.
* Yönlendirme (referral): Düşük — akademik ve blog ortaklıkları fırsat.

## Öneriler

* SEO konu kümeleri (topic clusters) oluştur: sure bazlı, tema bazlı (ahlak, hukuk, tarih) içerikler.
* Akademik işbirlikleri ve blog/yayıncılık ortaklıkları kurarak referral trafiğini artır.
* Sosyal strateji: kısa, dikkat-çekici alıntılar + okuma çağrısı; okuma başarıları (rozets) paylaşılabilir.

---

# KPI’lar ve 12–24 Ay Hedefleri (GA4 Uyumlu)

> Not: GA4 terminolojisini kullandık; ölçümlerin doğru çalışması için eventlerin tutarlı tanımları ve BigQuery’ye export önerilir.

## Ana KPI’lar

| KPI                         |            GA4 Karşılığı | 12 Ay Hedef | 24 Ay Hedef |
| --------------------------- | -----------------------: | ----------: | ----------: |
| Aylık Aktif Kullanıcı (MAU) |           `active_users` |        +%40 |       +%100 |
| Ortalama Oturum Süresi      |    `avg_engagement_time` |        +%25 |        +%50 |
| Tekrar Ziyaret Oranı        |       `returning_users%` |        +%20 |        +%40 |
| Sayfa / Oturum              |      `views_per_session` |        +%15 |        +%30 |
| Sosyal Trafik Payı          | `traffic_source: social` |        +%50 |       +%150 |

## Topluluk KPI’ları

* **Aktif geri bildirim:** `feedback_submit` — hedef ≥ %5 (tüm aktif kullanıcılara göre)
* **Seri tamamlama (multi-page read):** `series_continue` — hedef ≥ %30
* **30 gün geri dönüş (sadık okuyucu):** `return_30d` — hedef ≥ %35

---

# GA4 Event Taksonomisi ve Conversion Stratejisi

Aşağıdaki taksonomi, platformun özgün 'okuma odaklı' doğasına göre tasarlanmıştır. Her event için GA4'te `event_name`, event parametreleri ve önerilen event tetikleme mantığı verilmiştir.

> Uygulama notu: Event isimleri küçük harf, alttire (`_`) ile ayrılmış şekilde sabitlenmelidir. (örn. `read_complete`)

## 1) Okuma / Engagement Eventleri

| Event           | Tetikleme / Parametreler                                       | GA4 Kullanımı             |
| --------------- | -------------------------------------------------------------- | ------------------------- |
| `scroll_50`     | kullanıcı sayfada %50 scroll yaptığında                        | engagement ölçümü         |
| `scroll_90`     | %90 scroll                                                     | derin okuma ölçümü        |
| `read_30s`      | kullanıcı ≥30 sn sayfada görünür ise                           | mikro-dönüşüm             |
| `read_60s`      | ≥60 sn                                                         | daha güçlü mikro-dönüşüm  |
| `read_complete` | `read_60s` ve `scroll_90` kombinasyonu veya sayfa sonuna varış | ana dönüşüm (Derin Okuma) |

**Örnek gtag kodu (sayfa içinde):**

```js
// basit örnek (Next.js client side)
if(visibleTime >= 30) gtag('event','read_30s',{page_path: location.pathname});
if(scrollPercent >= 90) gtag('event','scroll_90',{page_path: location.pathname});
```

## 2) Gezinme ve Keşif Eventleri

* `internal_link_click` — iç link tıklamaları (source_page, dest_page parametreleri).
* `series_continue` — seri (multi-page) okumaya ilerleme (series_id, position).
* `topic_navigation` — konu etiketleri üzerinden gezinme (topic_id).

## 3) Geri Dönüş Eventleri

* `return_7d` — 7 gün içinde dönüş.
* `return_30d` — 30 gün içinde dönüş (Sadık Kullanıcı conversion'u için kullanılacak).

## 4) Katkı & Topluluk Eventleri

* `feedback_open` — geri bildirim paneli açılması.
* `feedback_submit` — geri bildirim gönderilmesi (type: correction/suggestion/opinion, content_length).
* `content_suggestion` — yeni içerik önerisi gönderimi.
* `comment_post` — ayet yorumu gönderimi.

## 5) İkincil Davranışsal Dönüşümler

* `bookmark_add` — yer imi ekleme.
* `share_click` — paylaşım butonuna tıklama (channel param).

## Conversion (Dönüşüm) Tanımları

**Ana Conversion’lar** (GA4 Conversion olarak işaretlenecek):

* `read_complete` — Derin Okuma (birincil hedef)
* `return_30d` — Sadık Kullanıcı
* `feedback_submit` — Aktif Katkı

**İkincil Conversion’lar**:

* `read_60s` — Okuma Eğilimi
* `series_continue` — İç Derinlik
* `feedback_open` — Katkı Niyeti

---

# Hunî (Funnel) Modeli ve Ölçüm Planı

## Önerilen Funnel

```
Ziyaretçi → read_30s → read_complete → return_7d → return_30d → feedback_submit
```

Her adımda düşüş oranlarını (drop-off) takip ederek, iyileştirme alanları belirleyin. Örneğin:

* Eğer `read_30s → read_complete` geçişi zayıfsa, içerik düzeni ve okunabilirlik kontrol edilmeli.
* `read_complete → return_7d` zayıfsa, push bildirimleri ve kişiselleştirilmiş e-posta hatırlatmaları devreye sokulmalı.

## Ölçüm Uygulama Notları

* Tüm eventlerin parametreleri standartlaştırılmalı: `page_id`, `series_id`, `user_id (anon)`, `topic`, `source`.
* BigQuery export etkinleştirilmeli; daha derin analiz ve segmentasyon için raw event export şart.
* Event etiketleri (GA4) ile Supabase'deki kullanıcı/puan verisi eşleştirildiğinde (anonim id mapping) gelişmiş cohort analizleri yapılabilir.

---

# Teknik İnceleme — Mevcut Durum ve Karşılaştırma

## Mevcut Altyapı (Özet)

* Frontend: Next.js 14.2 + TypeScript + Tailwind (PWA destekli)
* Backend / DB: Supabase (Postgres)
* Auth: Clerk
* Dağıtım: Vercel
* Diğer: Service Worker (PWA), Icecast Live Radio, Namaz-vakit proxy

## Karşılaştırma: quran.com ve kuran.diyanet.gov.tr

* **quran.com:** Teknik açıdan çok güçlü hızlı arama/filtreleme, çoklu meal, audio player. Ancak topluluk temelli yorum/etkileşim yok.
* **kuran.diyanet.gov.tr:** Resmî ve otoriter kaynak; bilgi zengin ama modern UX ve etkileşim açısından zayıf.

**Kur'ancılar avantajları:** Topluluk etkileşimi, sade modern arayüz, sosyal/oyunlaştırma imkanları.

---

# Geliştirme Önerileri ve Yol Haritası (Roadmap)

Aşağıda kısa dönem (0–3 ay), orta dönem (3–9 ay) ve uzun dönem (9–24 ay) öncelikleri bulabilirsiniz.

## 0–3 Ay (Hızlı Kazançlar)

* GA4: Event taksonomisini uygulama ve BigQuery exportu açma.
* `read_complete` ve `feedback_submit` eventleri canlıya alınıp Conversion olarak işaretlenmeli.
* Kritik performans optimizasyonu: Font yükleme, ilk içerik boyası (FCP) iyileştirmeleri.
* Basit push bildirimleri (namaz + haftalık okuma hatırlatması) için altyapı kur.
* Sosyal paylaşım butonları + meta etiket iyileştirmesi (OG tags) — trafik artışı için.

## 3–9 Ay (Büyüme ve Ürünleşme)

* Okuma serileri ve seviye/rozetsistemi uygulama.
* Abonelik altyapısı (Clerk + ödemeler) ve reklamsız paket.
* Moderasyon + itibar sistemi (yorumlara puan/veri doğrulama).
* Akademik işbirlikleri ve referral stratejileri başlatma.

## 9–24 Ay (Olgunlaşma ve Sürdürülebilirlik)

* Özelleşmiş mobil uygulama (native) ve PWA derinleştirme.
* İçerik yayılımı: çoklu meal entegrasyonları, tefsir derinliği.
* Büyüklük arttıkça Supabase ölçekleme (read replicas veya managed PG plan upgrade).
* Veri-odaklı ürünler: haftalık okuma raporları, kişiselleştirilmiş keşif.

---

# Mali Analiz ve Sürdürülebilirlik

**Mevcut Tahmin (Rapor verileri):**

* Aylık sabit gider (şirketli): ~20.000 TL (Muhasebe, Bağ-Kur, Vercel, Apple dev, alan adı vb.)
* İlk yıl hedef MAU: 1.000–2.000 (muhafazakâr)

## Gelir Modeli Özetleri

### Reklam

* Türkiye CPM ortalaması varsayımı: 25 TL
* İlk yıl gerçekçi reklam hedefi: 5.000–8.000 TL / ay (200–320k gösterim gerektirir)

### Abonelik (Reklamsız)

* Aylık ücret önerisi: 49 TL
* 200 abone → 9.800 TL
* 300 abone → 14.700 TL
* 400 abone → 19.600 TL

### Dengeli Hibrit Senaryo

* Reklam: 6.000 TL
* Abonelik (300 üye): 14.700 TL
* Toplam: 20.700 TL → aylık asgari maliyetin üzerine çıkar.

## Öneriler

* Abonelik faydasını (reklamsız + gelişmiş filtreleme + offline + premium rapor) net kılın.
* İlk 12 ayda promosyon/özel üyelik fiyatlarıyla 300 abone hedefi konulmalı.

---

# Topluluk, Moderasyon ve İçerik Yönetimi Politikası

## İlkeler

* Açık, saygılı tartışma ortamı sağlanmalı.
* Moderasyon **şeffaf** ve **kademeli** olmalı.

## Uygulanabilir Kurallar

* Yorumlar: hakaret, nefret ve yanlış bilgilendirme yasak.
* Geri bildirimler değerlendirilmeli; kabul edilen katkılar görünür şekilde teşekkür/aktarılmalı.
* İtibar sistemi: aktif katkılar puanlandırılmalı, yüksek puanlı katkılar öne çıkarılmalı.

## Moderasyon İş Akışı

1. Otomatik filtreleme (küfür/nefret anahtar kelimeler).
2. Topluluk raporu.
3. İnsan moderatör incelemesi (gönüllüler + core ekip).

---

# Operasyonel ve Güvenlik Önerileri

* **RLS (Row Level Security):** Supabase üzerinde herkesin yalnızca yetkili verileri görmesini sağlayın.
* **VAPID & Push Güvenliği:** Web push için VAPID anahtarları güvenli şekilde saklanmalı (server-side env var).
* **Yedekleme & Export:** Haftalık DB yedeği; BigQuery exportu sürekli event analizleri için.
* **GDPR/TKV:** Kişisel veriler için saklama politikası, kullanıcı veri talebi akışı dokümante edilmeli.

---

# Uygulanabilir Eylem Adımları — Hemen Yapılabilecekler

1. **GA4 event taksonomisini uygulamaya al** (öncelik: `read_30s`, `read_60s`, `scroll_90`, `read_complete`, `feedback_submit`).
2. **BigQuery export** aktif et.
3. **Push bildirim altyapısını** basit hatırlatmalar için aç (namaz + haftalık okuma önerisi).
4. **Abonelik sayfası** hazırla — temel paket; A/B testiyle teklif doğrula.
5. **Performans quick-win**: font optimizasyonu, critical CSS, next/image kontrolleri.
6. **Sosyal içerik kitleri**: paylaşılabilir kısa alıntılar, Open Graph iyileştirmeleri.

---

# Ekler — Teknik Detaylar ve Referanslar

## Veritabanı (Kısa Özet)

* `profiles` (clerk_id, display_name, score, streak, city, notification_settings)
* `comments` (id, ayet_id, user_id, content, parent_id, created_at)
* `forum_posts`, `forum_comments`, `post_likes`, `comment_likes`
* `push_subscriptions`, `notifications`

## API Örnekleri

* `GET /api/sure` — tüm sureler
* `GET /api/sure/[id]` — sure detay
* `POST /api/user/bookmark` — yer imi yönetimi
* `POST /api/push/subscribe` — push aboneliği

## .env Örnek

```
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=pk_test_...
CLERK_SECRET_KEY=sk_test_...
NEXT_PUBLIC_SUPABASE_URL=https://...
NEXT_PUBLIC_SUPABASE_ANON_KEY=ey...
NEXT_PUBLIC_VAPID_PUBLIC_KEY=...
VAPID_PRIVATE_KEY=...
VAPID_SUBJECT=mailto:admin@example.com
```

## GA4 Event Örnekleri (Snippet)

```js
// Scroll yüzde hesabı
window.addEventListener('scroll', ()=>{
  const doc = document.documentElement;
  const scrollPercent = (window.scrollY + window.innerHeight) / doc.scrollHeight * 100;
  if(scrollPercent >= 90 && !window._sent_scroll_90){
    gtag('event','scroll_90',{page_path: location.pathname});
    window._sent_scroll_90 = true;
  }
});

// Görünürlük (visibility API) ile read_30s
let visibleTime = 0; let interval;
function startTimer(){ interval = setInterval(()=>{ visibleTime +=1; if(visibleTime === 30) gtag('event','read_30s',{page_path: location.pathname}); if(visibleTime === 60) gtag('event','read_60s',{page_path: location.pathname}); },1000);}
function stopTimer(){ clearInterval(interval);}

document.addEventListener('visibilitychange', ()=>{
  if(document.visibilityState === 'visible') startTimer(); else stopTimer();
});
startTimer();
```

---

# Sonuç ve Kapanış

Kur'ancılar, teknik altyapı ve topluluk değeri bakımından güçlü bir başlangıç pozisyonunda. Uzun vadeli hedefler, ölçülebilir kullanıcı sadakati ve sürdürülebilir gelir modeline odaklanmalıdır. Bu raporda önerilen GA4 taksonomisi, conversion tanımları, hızlı yol haritası ve mali senaryolar hayata geçirildiğinde platform; niteliksel olarak benzersiz, niceliksel olarak ise sürdürülebilir bir noktaya ulaşacaktır.

---

*Hazırlayan: Yasir Eymen Kayabaşı*
