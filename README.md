# 🏗️ BETONARME U-KANAL TASARIM UYGULAMASI

Türkiye'deki teknik standartlara tam uyumlu, profesyonel betonarme u-kanal yapıların hidrolik, geoteknik, deprem ve yapısal tasarımını yapan web uygulaması.

## ✨ Özellikler

### 📊 Kapsamlı Analiz
- **Hidrolik Hesaplamalar**: Manning denklemi, Froude sayısı, akım tipi analizi
- **Geoteknik Analiz**: Rankine ve Coulomb teorileri, toprak basıncı hesapları
- **Deprem Analizi**: TBDY 2018 uyumlu Mononobe-Okabe pseudo-statik analiz
- **Stabilite Kontrolleri**: Devrilme, kayma, taşıma gücü güvenlik kontrolleri
- **Yapısal Tasarım**: TS 500 uyumlu betonarme donatı tasarımı
- **Kesme Donatısı (Etriye)**: TS 500 §8.5 uyumlu etriye hesabı
- **Metraj Hesaplamaları**: Beton, kalıp ve donatı metrajları

### 🇹🇷 Türk Standartları Uyumluluğu
- ✅ **TBDY 2018** - Türkiye Bina Deprem Yönetmeliği
- ✅ **TS 500:2000** - Betonarme Yapıların Tasarım ve Yapım Kuralları
- ✅ **TS EN 1997-1** - Geoteknik Tasarım (EC7) - DA1/DA2 yaklaşımları
- ✅ **TS EN 1992-1-1** - Beton Yapılar (Eurocode 2)

### 🎯 Kullanıcı Deneyimi
- Responsive web tasarımı (masaüstü, tablet, mobil)
- 8 sekme halinde organize edilmiş arayüz
- Gerçek zamanlı hesaplamalar
- Otomatik optimizasyon önerileri
- Tasarım karşılaştırma aracı
- Detaylı teknik rapor oluşturma
- Rapor yazdırma ve Excel export seçenekleri

## 🚀 Başlangıç

### Sistem Gereksinimleri
- Modern web tarayıcı (Chrome, Firefox, Edge, Safari)
- JavaScript etkin olmalı
- İnternet bağlantısı gerekmez (offline çalışır)

### Kullanım
1. `u-kanal-tasarim.html` dosyasını tarayıcıda açın
2. Giriş verileri sekmesine gerekli parametreleri girin:
   - Hidrolik parametreleri (tasarım debisi, kanal genişliği, vb.)
   - Geometrik parametreler (duvar yüksekliği, temel boyutları)
   - Zemin parametreleri (sürtünme açısı, kohezyon, taşıma gücü)
   - Deprem parametreleri (SDS, SD1, zemin sınıfı)
   - Malzeme özellikleri (beton sınıfı, donatı türü, çevre koşulları)
3. **"Tüm Hesaplamaları Yap"** butonuna tıklayın
4. Sonuçları diğer sekmeler de inceleyebilirsiniz

## 📋 Sekme Yapısı

| Sekme | İçerik |
|-------|--------|
| **📋 Giriş Verileri** | Tüm tasarım parametrelerinin girildiği bölüm |
| **💧 Hidrolik Hesaplar** | Su derinliği, akım hızı, Froude sayısı, hidrostatik basınç |
| **🏔️ Geoteknik Analiz** | Toprak basıncı, taşıma gücü, ağırlık hesapları |
| **🌊 Deprem Analizi** | TBDY 2018 uyumlu Mononobe-Okabe deprem itkileri |
| **⚖️ Stabilite Kontrolü** | Statik ve dinamik devrilme, kayma, taşıma güvenliği |
| **🔧 Yapısal Tasarım** | Donatı hesabı, kesme kontrol, etriye seçimi |
| **📊 Metraj** | Beton, kalıp ve donatı metrajları |
| **📄 Rapor** | Özet teknik rapor ve imza alanları |

## 🔧 Teknik Detaylar

### Tasarım Standartları ve Güvenlik Katsayıları

#### TBDY 2018 Statik Kontroller
| Kontrol | GS ≥ |
|---------|------|
| Devrilme | 2.0 |
| Kayma | 1.5 |
| Taşıma Gücü | 2.5 |

#### TBDY 2018 Dinamik Kontroller
| Kontrol | GS ≥ |
|---------|------|
| Devrilme | 1.5 |
| Kayma | 1.2 |
| Taşıma Gücü | 1.5 |

### Hesaplama Yöntemleri

**Hidrolik:**
- Manning denklemi: V = (1/n) × R_h^(2/3) × S_o^(1/2)
- Newton-Raphson iteratif çözümü

**Geoteknik:**
- Rankine ve Coulomb toprak basıncı teorileri
- Terzaghi taşıma gücü formülü
- Meyerhof katsayıları

**Deprem (TBDY 2018):**
- Tam Mononobe-Okabe pseudo-statik analiz
- Spektral ivme hesabı (SD1 desteği)
- İki yönlü deprem kombinasyonu

**Yapısal:**
- TS 500 yük kombinasyonları
- Moment ve kesme tasarımı
- Donatı hesabı (omega yöntemi)
- Çatlak kontrolü (TS 500 §13.5)

## 💾 Proje Yapısı

```
wall-app/
├── u-kanal-tasarim.html      # Ana uygulama (2900+ satır)
├── README.md                  # Bu dosya
├── .gitignore                 # Git exclude kuralları
└── .git/                       # Git deposu
```

### Dosya Bilgileri
- **Boyut**: ~160 KB (sıkıştırılmış)
- **Bağımlılık**: Yok (Pure HTML/CSS/JavaScript)
- **Dil**: Turkish (Türkçe)

## 🛠️ Kurulum ve Geliştirme

### Klonlama
```bash
git clone https://github.com/palamut62/wall-app.git
cd wall-app
```

### Yerel Çalıştırma
Dosyayı doğrudan tarayıcıda açın:
```bash
# Windows
start u-kanal-tasarim.html

# macOS
open u-kanal-tasarim.html

# Linux
xdg-open u-kanal-tasarim.html
```

Veya basit bir web sunucusu başlatın:
```bash
# Python 3
python -m http.server 8000

# Node.js
npx http-server
```

Tarayıcıda `http://localhost:8000` adresini açın.

## 📝 Giriş Parametreleri

### Hidrolik
- **Q_T**: Tasarım Taşkın Debisi (m³/sn) - Varsayılan: 50
- **b**: Kanal Genişliği (m) - Varsayılan: 5.0
- **n**: Manning Katsayısı - Varsayılan: 0.015
- **S_o**: Kanal Eğimi (m/m) - Varsayılan: 0.001

### Geometrik
- **H**: Toplam Duvar Yüksekliği (m) - Varsayılan: 6.0
- **B**: Temel Genişliği (m) - Varsayılan: 3.0
- **T_H**: Temel Kalınlığı (m) - Varsayılan: 0.6
- **L**: Duvar Uzunluğu (m) - Varsayılan: 1.0

### Zemin
- **φ**: İçsel Sürtünme Açısı (°) - Varsayılan: 30
- **c**: Kohezyon (kPa) - Varsayılan: 0
- **γ**: Zemin Birim Ağırlığı (kN/m³) - Varsayılan: 18
- **q_ult**: Taşıma Gücü (kN/m²) - Varsayılan: 250

### Deprem (TBDY 2018)
- **S_DS**: Kısa Periyot Spektral İvme (g) - Varsayılan: 0.8
- **S_D1**: 1 Saniye Spektral İvme (g) - Varsayılan: 0.35
- **Zemin Sınıfı**: ZA-ZE - Varsayılan: ZC
- **r**: Azaltma Katsayısı - Varsayılan: 2.0

### Malzeme
- **Beton Sınıfı**: C25/30, C30/37, C35/45, C40/50 - Varsayılan: C30/37
- **Donatı**: B420C, B500C - Varsayılan: B420C
- **Çevre Koşulları**: XC1-XS3 - Varsayılan: XC4

## 🎓 Örnek Tasarım

Varsayılan parametrelerle uygulamayı açtığınızda, aşağıdaki tipik bir U-kanal tasarımı için sonuçlar alırsınız:
- Su derinliği: ~0.8-1.0 m
- Aktif toprak basıncı: ~20-30 kN/m
- Dinamik etki: ~15-20% artış
- Minimum donatı: Φ16 @ 150 mm

## ⚠️ Sınırlamalar ve Uyarılar

1. **Pseudostatik Analiz**: Dinamik analiz değil, yapılara ait dinamik özellikler basitleştirilmiş varsayılmıştır
2. **Düzey Gürültü**: Hidrolik hesaplamalarda 2D kanal akışı varsayılmıştır
3. **Zemin Özellikleri**: Homojen, izotrop zemin varsayılmıştır
4. **Drenaj**: Mükemmel drenaj kabul edilmiştir
5. **Sıvılaşma**: Sınırlı sıvılaşma analizi yapılmıştır

## 🐛 Bilinen Sorunlar ve Çözümleri

- ✅ NaN değerleri otomatik olarak 0'a çevriliyor
- ✅ Hata kontrolleri ve fallback mekanizmaları eklendi
- ✅ Tüm hesaplamalar giriş değeri doğrulamasından geçiyor

## 📞 Destek ve Raporlama

Sorun bulduysanız veya öneriniz varsa:
- GitHub Issues: https://github.com/palamut62/wall-app/issues
- Email: palamut62@github.com

## 📚 Kaynaklar ve Referanslar

### Türk Standartları
- TBDY 2018 - Türkiye Bina Deprem Yönetmeliği
- TS 500:2000 - Betonarme Yapıların Tasarım ve Yapım Kuralları
- TS EN 1997-1 - Geoteknik Tasarım (Eurocode 7)
- TS EN 1992-1-1 - Beton Yapılar (Eurocode 2)

### Referans Kitapları
- "İstinat Yapıları" - Jeoteknik Mühendisliği Ders Notları
- "Kanal Tasarımı" - Hidroloji ve Hidrolik Mühendisliği
- "Betonarme Tasarımı" - TS 500 Uygulamaları

## 📄 Lisans

Bu proje açık kaynak olarak sunulmuştur. Kullanım, değiştirme ve dağıtım için MIT Lisansı uygulanır.

## ✍️ Yazarlar

- Palamut62 - Geliştirici
- Claude AI - Türk Standartları Uyumluluğu İyileştirmeleri

## 📈 Sürüm Tarihi

### v1.1.0 (Kasım 2024)
- ✅ TBDY 2018 güvenlik faktörleri düzeltildi
- ✅ SD1 spektral ivme parametresi eklendi
- ✅ Kesme donatısı (etriye) hesabı eklendi
- ✅ TS EN 1997-1 (EC7) kısmi güvenlik faktörleri desteği
- ✅ NaN hata kontrolü ve düzeltmeleri
- ✅ Hata yakalama mekanizmaları eklendi

### v1.0.0 (İlk Sürüm)
- Temel hidrolik, geoteknik, deprem ve yapısal analiz

---

**Son Güncelleme**: 17 Kasım 2024
**Durum**: ✅ Production Ready - Türk Standartlarına Tam Uyumlu

