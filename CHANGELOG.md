# Değişiklik Günlüğü

Bu dosya, kitabın sürümler arasındaki önemli değişikliklerini takip eder.

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

### Ek güncellemeleri
- **Ek A — Sayı Sistemleri ve Kodlama** kapsamlı güncelleme
  - Göbekli Tepe bölüm fotoğrafı eklendi
  - İçerik genişletildi ve yeniden yapılandırıldı
- **Ek B — Sayısal Tasarım Temelleri** güncellemeleri
  - Galata Kulesi bölüm fotoğrafı eklendi
  - Giriş, kısaltmalar listesi ve örnekler iyileştirildi

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
