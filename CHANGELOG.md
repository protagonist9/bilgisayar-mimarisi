# Değişiklik Günlüğü

Bu dosya, kitabın sürümler arasındaki önemli değişikliklerini takip eder.

---

## [0.3.5] — 2026-03-19

### Yeni bölüm
- **Bölüm 4 — RISC-V ile Programlama** eklendi
  - Temel aritmetik ve bellek erişim örnekleri (yığıta okuma/yazma, bellek işlemleri)
  - Yığıt kullanımı: yazmaç saklama, altyordam çağrıları, yığıt çerçevesi
  - Döngüler ve dallanma: toplam hesaplama, doğrusal arama, kabarcık sıralama
  - Karakter dizisi işleme: strlen, strcpy, palindrom (çevirmece)
  - Yapılar ve bağlı listeler: bellek düzeni, hizalama, düğüm gezinme
  - Özyineleme: Fibonacci, çağrı ağacı TikZ şekli, yığıt büyümesi TikZ şekli
  - Çok fonksiyonlu programlar: yaprak/yaprak olmayan ayrımı
  - Kod eniyileme: güç azaltma, döngü açma, matris işleme
  - Donanım etkileşimi: MMIO LED, UART seri iletişim
  - Başarım çözümlemesi: buyruk sayımı, BBÇ hesabı, bellek erişim oranı
  - Hata ayıklama ve yaygın yanılgılar
  - 24 çözümlü örnek, 6 TikZ şekli, yazmaç izleme tabloları, 30 alıştırma

### Bölüm numaralandırması
- Bölüm 4 eklenmesiyle eski bölümler yeniden numaralandırıldı (eski 4→5, 5→6, ..., 11→12)

### Bölüm 1 — Yeni içerik
- **Dört Tasarım İlkesi** alt bölümü eklendi: küçük olan hızlıdır, olağan durumu hızlandır, ödünleşme, yalınlık düzenden gelir
- **Bilgi Notu**: "Tasarım İlkeleri Yalnızca Donanım İçin mi?" — günlük hayat örnekleri ve YouTube video bağlantısı
- **Örnek 1.6** (yeni): Dennard ölçeklemesi nicel hesaplama — iki kuşak işlemci karşılaştırması
- **Moore yasası tartışma sorusu** (yeni alıştırma)
- Eski Örnek 1.6 (MTTF) → Örnek 1.7 olarak yeniden numaralandırıldı
- Çapraz referanslar eklendi (güç tüketimi→B6/B7, yazılım katmanları→B3/B4, güvenilirlik→B8/B9)

### Bölüm 2 — Yeni içerik
- **Yeni şekil**: Amdahl Yasası hızlanma eğrileri (pgfplots, 5 koşut oran)
- **Yeni şekil**: Gecikme vs işlem hacmi karşılaştırma diyagramı
- **Örnek 2.14** (yeni): Enerji-gecikme çarpımı (EDP) çözümlü örneği — DVFS bağlantısı
- **2 yeni alıştırma**: Amdahl yasası web tarayıcısı (3 senaryo) + SPEC CPU2017 geometrik ortalama
- Çapraz referanslar eklendi (Amdahl→B7, saat çevrimi→B6)

### Bölüm 3 — Yeni içerik ve şekil iyileştirmeleri
- **Örnek 3.20** (yeni): Adresleme kipleri çözümlü sayısal örnek (5 buyruk, tüm kipler)
- **Yeni TikZ şekli**: İç içe altyordam çağrısında çağıran/çağrılan yığıt çerçeveleri
- Adresleme kipi şekilleri (3.14--3.18) Şekil 3.11 buyruk biçimi stiliyle tutarlı hale getirildi
- Bit numaraları tüm adresleme kipi şekillerine eklendi

### Bölüm 4 — Ek içerik
- **Yeni TikZ şekli**: Fibonacci n=4 yığıt çerçevelerinin birikmesi (yığıt tepesi yukarıda)
- **auipc bilgi notu**: PS değeri ve konumdan bağımsız kod mekanizması
- **17 yeni alıştırma** (13→30): C→RISC-V dönüşümleri, yazmaç kuralları, yığıt analizi, hata ayıklama, başarım
- Çapraz referanslar eklendi (derleyici→B7, bellek→B8, başarım→B2)

### Ek D — İyileştirmeler
- **10 yeni alıştırma** (0→10): RARS çalıştırma, Verilog modül tasarımı, yazmaç öbeği genişletme, önbellek analizi
- **2 yeni TikZ şekli**: Yazmaç öbeği blok diyagramı, Verilog modül hiyerarşisi
- "Yazmaç Dosyası" → "Yazmaç Öbeği" terminoloji düzeltmesi
- "Testbench" → "Doğrulama ortamı" terminoloji düzeltmesi

### Altyapı
- **Sürüm yönetimi yeniden yapılandırıldı**: `surum-ayarlari.tex` merkezi kontrol dosyası
- `\bolumekle` / `\ekekle` makroları: dosya varsa include, yoksa otomatik atla
- `\kitapsurum` komutu: sürüm numarası tek yerden yönetiliyor
- İçindekiler'e Şekil Listesi ve Tablo Listesi eklendi
- Kapak sonrası boşluk düzeltildi (cleardoublepage → clearpage)
- İthaf sayfası: fotoğraf büyütüldü (0.85→0.95), dikey ortalama
- `\lstlistingname` → "Kod" (Listing → Kod)

### Terminoloji
| Eski kullanım | Yeni kullanım |
|---|---|
| mobil | taşınabilir |
| alternatif | seçenek |
| yazmaç dosyası | yazmaç öbeği |
| Testbench | Doğrulama ortamı |
| Listing | Kod |

### Hata düzeltmeleri
- Bölüm 2: `sinyalsari` tanımsız renk → `orange!20` ile değiştirildi
- Bölüm 2: lstlisting içinde `&` → `adres()` ile değiştirildi
- Referanslar [0] sorunu çözüldü (biber tam derleme sırası)

---

## [0.3.0] — 2026-03-16

### Yeni bölüm
- **Bölüm 3 — Buyruk Kümesi Mimarisi** eklendi
  - Buyruk kümesi mimarisi (BKM) tasarım ilkeleri ve kısa tarihçe
  - RISC-V işlemcisi ve buyruk kümesine giriş
  - Yazmaçlar: türleri, RISC-V yazmaç dosyası, sıfır yazmacı (x0), yazmaç sayısı ödünleşme tartışması
  - Bellek düzeni: sözcük kavramı, bellek erişim türleri, hizalama, bayt sırası (endianness)
  - Buyruk türleri (R/I/S/B/U/J) ve kodlama biçimleri
  - Veri aktarma, aritmetik, mantık, kaydırma, dallanma ve atlama buyrukları
  - Çarpma ve bölme: geniş sonuç sorunu
  - Sözde buyruklar
  - Adresleme kipleri (yazmaç, anlık, eklemeli, PS'ye göreceli, üst anlık)
  - Altyordam ve yığıtlar: çağrı kuralları, yığıt çerçevesi, iç içe çağrılar
  - Programın yürütülmesi: derleyici, çevirici, bağlayıcı, yükleyici, bellek düzeni, sistem çağrıları
  - Diğer BKM'ler: MIPS, ARM, x86 karşılaştırması
  - 19 çözümlü örnek, 22 şekil, 29 tablo, 16 karşılaştırma kutusu, 36 alıştırma

### Bölüm 2 — Yeni içerik
- **Heterojen Sistemlerde Başarım** alt bölümü eklendi
  - Tek yonga (SoC) blok diyagramı (yeni TikZ şekil)
  - Genişletilmiş Amdahl Yasası heterojen sistemler için
- Apple M serisi SoC açıklaması M1'den M5'e genişletildi
- BBÇ terimnotu kutusu yeniden formatlandı
- MIPS ve kayan nokta terim notları başlıkları güncellendi

### Ek C — Yeni içerik
- **C.7 Kodlama Örnekleri** bölümü eklendi (4 uçtan uca örnek: aritmetik, döngü, koşul, fonksiyon çağrısı)

### Preamble
- Yeni `karsilastirma` kutusu ortamı eklendi (diğer mimarilerle karşılaştırma için)

### Kaynakça
- 3 yeni referans: Hill & Marty 2008, Patterson & Ditzel 1980, Cohen 1980

### Terminoloji

| Eski kullanım | Yeni kullanım |
|---|---|
| hassasiyet | duyarlık |
| düşük duyarlık toleransı | düşük duyarlıkta yeterli doğruluk |
| yazmaç tahsisi | yazmaç ataması |
| isabet/ıskalama (önbellek) | bulma/bulamama |
| istisna (boru hattı) | kural dışı durum |
| fiilen | uygulamada |
| simüle etmek | benzetmek |

### Kapak
- "Sürüm 0.2.1" → "Sürüm 0.3.0"

---

## [0.2.1] — 2026-03-10

### Yeni ekler
- **Ek C — RISC-V Referans Kartı** eklendi
  - RV32I taban buyruk kümesi tablosu (R/I/S/B/U/J türleri)
  - Sözde buyruklar tablosu
  - Yazmaç adlandırma ve çağrı kuralları tablosu
  - Yığıt çerçevesi diyagramı (Şekil C.1)
  - CSR buyrukları ve bellek sıralama buyrukları
  - M, A, F, D uzantıları özet tabloları
  - Alıştırmalar (buyruk kodlama/çözme)

- **Ek D — Uygulamalı Çalışma Rehberi** eklendi
  - RARS ve Venus simülatörleri kurulum ve kullanım
  - Fibonacci örnek programı (doğrudan çalıştırılabilir)
  - Icarus Verilog / GTKWave kurulum rehberi
  - Verilog ile sayısal tasarım temelleri
  - SystemVerilog tanıtımı
  - Testbench yazımı ve dalga formu görüntüleme
  - FPGA ile gerçekleme bilgi notu
  - Mini projeler (ALU, yazmaç dosyası, bellek, basit işlemci)

- **Ek A — Sayı Sistemleri ve Kodlama** eklendi
  - Göbekli Tepe bölüm fotoğrafı
  - Taban dönüşümleri, işaretli sayı gösterimleri, karakter kodlama

### Terminoloji
- Ek C: Dallanma/atlama buyruklarında "ofset" → "eklenti" düzeltmesi (bellek adresleme "ofset" korundu)
- Terimler sözlüğüne "benzetim/benzetimlik" (simulation/simulator) eklendi

### Kapak
- "Sürüm 0.2.0" → "Sürüm 0.2.1"

---

## [0.2.0] — 2026-03-09

### Yeni bölüm
- **Bölüm 2 — Bilgisayar Başarımı** eklendi
  - Başarım tanımı ve gereksinim belirleme
  - Saat sıklığı, çevrim zamanı ve çevrim sayısı
  - Buyruk Başına Çevrim (BBÇ) ve yürütme zamanı formülü
  - İşlem hacmi ve gecikme kavramları
  - FLOPS, SPEC ve sınama programları
  - Amdahl Yasası (tarihsel giriş, adım adım türetim) ve Gustafson Yasası
  - Güç-başarım dengesi ve enerji verimliliği
  - Tarihsel başarım eğilimleri (altın çağ, güç duvarı, bellek duvarı, çok çekirdekli dönem)
  - 12 çözümlü örnek, 34 alıştırma

### Bölüm 1 güncellemeleri
- **Makine Dili ve Çevirici Dil** alt bölümü genişletildi: işlem kodu/işlenen yapısı, RISC-V `add x5, x6, x7` buyruğunun montaj dili → ikili → onaltılık dönüşüm tablosu
- **Von Neumann ve Harvard Mimarileri** alt bölümü genişletildi: EDVAC raporuna tarihsel atıf, Von Neumann darboğazı açıklaması, değiştirilmiş Harvard mimarisi; yan yana karşılaştırma şekli eklendi (Şekil 1.9)
- **RISC ve CISC Tasarım Felsefeleri** alt bölümü yeniden yazıldı: yükle-sakla mimarisi kavramı, `A = A + B[i]` somut karşılaştırması (CISC: 1 buyruk, RISC: 4 buyruk), 9 satırlık karşılaştırma tablosu (Tablo 1.4), mikro-işlem dönüşümü tartışması
- **Yazılım Katmanları** alt bölümü genişletildi: sistem/uygulama yazılımı ayrımı, işletim sistemi ve derleyici paragrafları, 5 katmanlı TikZ diyagramı (Şekil 1.11)
- Bölüm özeti ve yanılgılar bölümü güncellendi
- 8 yeni sayısal alıştırma eklendi (1.21–1.28): yonga üretimi, güç tüketimi, Moore Yasası
- Şekil 1.4 görselleri yeniden oluşturuldu (masaüstü, dizüstü, akıllı telefon, sunucu, gömülü sistem)

### Terminoloji
Kitap genelinde Türkçe terim kullanımı güçlendirildi:

| İngilizce | Eski kullanım | Yeni kullanım |
|---|---|---|
| analysis | analiz | çözümleme |
| CPU | CPU | MİB (merkezi işlem birimi) |
| critical | kritik | can alıcı |
| factor | faktör | etken |
| index | indeks | dizin |
| message | mesaj | ileti |
| parallel | paralel | koşut |
| throughput | verim | işlem hacmi |
| web | web | örün |

Her terim ilk geçtiği yerde bir **terim notu** kutusuyla açıklanmıştır.

### Kapak
- "Sürüm 0.1.0" → "Sürüm 0.2.0"

---

## [0.1.0] — 2026-03-07

### İlk sürüm
- Bölüm 1 (Giriş) yayınlandı
- Kapak sayfası tasarımı (TikZ, PCB arka plan)
- Lisans: CC BY-NC-ND 4.0
- GitHub public repo oluşturuldu
- Release PDF yayınlandı
