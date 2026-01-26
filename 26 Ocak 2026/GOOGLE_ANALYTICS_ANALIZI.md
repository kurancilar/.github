# Kur’ancılar Platformu  
## Google Analytics Analizi, KPI’lar ve GA4 Event & Conversion Stratejisi Raporu

**Platform:** kuran.yasireymen.com  
**Rapor Türü:** Stratejik Analiz & Kamuoyu Bilgilendirme  
**Zaman Ufku:** Uzun Vadeli (12–24 Ay)  
**Hedef Kitle:** İç ekip, gönüllü katkıcılar ve kamuoyu  

---

## 1. Amaç ve Kapsam

Bu raporun amacı:

- Kur’ancılar platformunun mevcut dijital performansını analiz etmek  
- Kullanıcı davranışlarını anlamlandırmak  
- Ölçülebilir ve sürdürülebilir büyüme hedefleri belirlemek  
- Şeffaf, izlenebilir ve geliştirilebilir bir analitik yapı oluşturmaktır  

Analiz; Google Analytics (GA4) üzerinden elde edilen şu veri gruplarına dayanmaktadır:

- Kullanıcı etkileşimi ve elde tutma  
- Trafik kaynakları  
- Kullanıcı özellikleri  
- Davranışsal dönüşümler  

---

## 2. Platformun Genel Karakteri

Kur’ancılar platformu:

- Tüketim odaklı değil, **okuma ve düşünme odaklıdır**
- Sosyal medya bağımlı değil, **organik ve doğrudan erişimlidir**
- Sessiz ama **yüksek sadakat potansiyeline sahip** bir kullanıcı kitlesine hitap eder  

Bu nedenle klasik ticari KPI’lar yerine **anlamlı etkileşim metrikleri** tercih edilmiştir.

---

## 3. Kullanıcı Etkileşimi ve Elde Tutma Analizi

### 3.1 Gözlemler

- Kullanıcılar siteye **amaçlı** gelmektedir  
- Oturum süreleri derin okuma davranışına işaret eder  
- İçerik tek seferlik değil, **referans niteliğindedir**

### 3.2 Risk ve Fırsat Tablosu

| Alan | Mevcut Durum | Yorum |
|---|---|---|
| İlk ziyaret | Güçlü | SEO uyumu yüksek |
| Tekrar ziyaret | Orta | Hatırlatma mekanizması eksik |
| Aktif katılım | Düşük | Araç ve yönlendirme ihtiyacı |

---

### Grafik 1 – Kullanıcı Elde Tutma Eğrisi (Temsili)

```

Kullanıcı Oranı
100% |■■■■■■■■■■
75% |■■■■■■■
50% |■■■■
25% |■■
----------------
Gün 1   Gün 7   Gün 30

```

---

## 4. Trafik Kaynakları Analizi

### 4.1 Trafik Dağılımı (Nitel)

| Kaynak | Göreli Pay | Stratejik Anlam |
|---|---|---|
| Organik Arama | Yüksek | İçerik doğru anahtar kelimelerde |
| Doğrudan | Yüksek | Sadık çekirdek kitle |
| Sosyal | Düşük | Genişleme alanı |
| Yönlendirme | Düşük | Akademik & blog açılımı mümkün |

### Grafik 2 – Trafik Kaynakları Dağılımı

```

Organik       ████████████████
Doğrudan      ████████████
Sosyal        ███
Yönlendirme   ██

```

---

## 5. Kullanıcı Özellikleri (Profil)

- Mobil kullanım ağırlıklıdır  
- Modern tarayıcılar yaygındır  
- Türkiye merkezli, diaspora erişimine açıktır  

**Sonuç:**  
Hız, okunabilirlik ve düşük veri tüketimi kritik önemdedir.

---

## 6. Somut KPI Tablosu (GA4 Uyumlu)

### 6.1 Ana KPI’lar

| KPI | GA4 Karşılığı | 12 Ay Hedef | 24 Ay Hedef |
|---|---|---|---|
| Aylık Aktif Kullanıcı (MAU) | Active users | +%40 | +%100 |
| Ortalama Oturum Süresi | Avg. engagement time | +%25 | +%50 |
| Tekrar Ziyaret Oranı | Returning users % | +%20 | +%40 |
| Sayfa / Oturum | Views per session | +%15 | +%30 |
| Sosyal Trafik Payı | Traffic source: Social | +%50 | +%150 |

### 6.2 Topluluk KPI’ları

| KPI | Tanım | Hedef |
|---|---|---|
| Aktif geri bildirim | Katkı gönderen kullanıcı | ≥ %5 |
| Seri tamamlama | Çoklu sayfa okuma | ≥ %30 |
| 30 gün geri dönüş | Sadık okuyucu | ≥ %35 |

---

## 7. GA4 Event Taksonomisi

### 7.1 Okuma Event’leri

| Event | Tetik |
|---|---|
| scroll_50 | %50 scroll |
| scroll_90 | %90 scroll |
| read_30s | ≥30 sn |
| read_60s | ≥60 sn |
| read_complete | Süre + scroll |

### 7.2 Gezinme Event’leri

| Event |
|---|
| internal_link_click |
| series_continue |
| topic_navigation |

### 7.3 Geri Dönüş Event’leri

| Event |
|---|
| return_7d |
| return_30d |

### 7.4 Katkı Event’leri

| Event |
|---|
| feedback_open |
| feedback_submit |
| content_suggestion |

---

## 8. Conversion (Dönüşüm) Tanımları

### 8.1 Ana Conversion’lar

| Conversion | Event |
|---|---|
| Derin Okuma | read_complete |
| Sadık Kullanıcı | return_30d |
| Aktif Katkı | feedback_submit |

### 8.2 İkincil Conversion’lar

| Conversion | Event |
|---|---|
| Okuma Eğilimi | read_60s |
| İç Derinlik | series_continue |
| Katkı Niyeti | feedback_open |

---

## 9. GA4 Funnel (Hunî) Modeli

```

Ziyaretçi
↓
read_30s
↓
read_complete
↓
return_7d
↓
return_30d
↓
feedback_submit

```

---

## 10. Uzun Vadeli Büyüme Stratejisi

### 10.1 Kullanıcı Büyümesi
- SEO konu kümeleri
- İç bağlantı derinliği

### 10.2 Etkileşim Derinliği
- Seri içerikler
- Okuma ilerleme göstergeleri

### 10.3 Topluluk Oluşumu
- Düşük bariyerli katkı
- Şeffaf değişiklik kayıtları

---

## 11. Sonuç

Kur’ancılar platformu:

- Popülerlik değil **sadakat**
- Tıklama değil **okuma**
- Sayı değil **davranış**

üzerinden büyümeyi hedefleyen bir dijital düşünce platformudur.

Bu rapor, söz konusu büyümenin analitik temelini oluşturmaktadır.
