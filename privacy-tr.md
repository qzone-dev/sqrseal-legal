---
title: SQRSeal Gizlilik Politikası
---
**Son güncelleme:** Haziran 2026  
**Yürürlük tarihi:** Haziran 2026

---

## 1. Giriş

SQRSeal ("uygulama", "biz"), kullanıcılarının dijital güvenliğini korumayı amaçlayan bir URL ve QR kod güvenlik analiz uygulamasıdır. Bu Gizlilik Politikası, uygulamamızı kullandığınızda hangi verilerin toplandığını, nasıl kullanıldığını ve haklarınızı açıklamaktadır.

Uygulamayı kullanarak bu politikayı kabul etmiş sayılırsınız. Kabul etmiyorsanız lütfen uygulamayı kullanmayınız.

---

## 2. Toplanan Veriler

### 2.1 Otomatik Olarak Toplanan Veriler

**Anonim Cihaz Kimliği**
- Uygulamanın ilk açılışında rastgele bir cihaz kimliği oluşturulur.
- Bu kimlik cihazınızda saklanır ve Supabase sunucularımıza iletilir.
- Adınız, e-posta adresiniz veya telefon numaranız gibi kişisel kimlik bilgilerinizle ilişkilendirilmez.
- Uygulamayı yeniden yüklerseniz yeni bir kimlik oluşturulur.

**Sorgulanan URL ve Domain Bilgisi**
- Güvenlik analizi için girdiğiniz, taradığınız veya panodan yakalanan URL'lerin domain bilgisi sunucularımıza iletilir.
- URL'ler güvenlik tehditlerini tespit etmek amacıyla işlenir.
- Kişisel içerik veya hassas bilgi içeren URL'leri sorgulamaktan kaçınmanızı öneririz.

**Sorgu İstatistikleri**
- Toplam sorgu sayısı, tehdit tespiti sonuçları ve tarama kaynağı (manuel, QR, OCR, pano) kaydedilir.
- Bu veriler yalnızca size ait istatistikleri göstermek için kullanılır.

**Teknik Performans Verileri**
- Yanıt süresi (ms), önbellek kullanımı ve ağ bağlantı bilgileri toplanır.
- Bu veriler uygulamanın performansını iyileştirmek amacıyla kullanılır ve sizi tanımlamak için kullanılmaz.

**Uygulama Olayları**
- Bağlantı açma, OCR tarama gibi uygulama içi olaylar anonim olarak kaydedilir.
- Bu veriler ürün geliştirme amacıyla kullanılır.

### 2.2 Toplanmayan Veriler

Aşağıdaki veriler **kesinlikle toplanmaz:**
- Ad, soyad, e-posta adresi, telefon numarası
- Konum bilgisi
- Fotoğraf, kamera görüntüsü (OCR analizi sırasında yüklenen görseller işlendikten sonra otomatik silinir)
- Pano içeriği (yalnızca URL içerip içermediği kontrol edilir; URL değilse işlem yapılmaz)
- Sosyal medya veya hesap bilgileri

---

## 3. Verilerin Kullanım Amacı

Toplanan veriler yalnızca şu amaçlarla kullanılır:

| Amaç | Veri |
|------|------|
| URL güvenlik analizi sağlamak | Domain bilgisi |
| Kişisel sorgu geçmişini göstermek | Sorgu kayıtları |
| Uygulama performansını ölçmek | Teknik metrikler |
| Hataları tespit edip düzeltmek | Crash raporları |
| Ürün geliştirme kararları almak | Anonim kullanım istatistikleri |

Verileriniz üçüncü taraflara satılmaz, kiralanmaz veya ticari amaçlarla paylaşılmaz.

---

## 4. Üçüncü Taraf Hizmetleri

SQRSeal, güvenlik analizini gerçekleştirmek için aşağıdaki üçüncü taraf hizmetlerinden yararlanmaktadır. Her hizmet kendi gizlilik politikasına tabidir.

### 4.1 Google Web Risk API
- **Amaç:** URL'lerin bilinen tehdit veritabanlarına karşı kontrol edilmesi
- **İletilen veri:** Sorgulanan URL
- **Gizlilik politikası:** https://policies.google.com/privacy

### 4.2 URLScan.io
- **Amaç:** URL'lerin daha derin güvenlik analizi için taranması
- **İletilen veri:** Sorgulanan URL
- **Gizlilik politikası:** https://urlscan.io/about/#privacy

### 4.3 Supabase
- **Amaç:** Veritabanı ve sunucu altyapısı
- **İletilen veri:** Anonim cihaz kimliği, sorgu kayıtları
- **Veri merkezi:** Avrupa Birliği
- **Gizlilik politikası:** https://supabase.com/privacy

### 4.4 Sentry
- **Amaç:** Uygulama hata takibi ve crash raporlama
- **İletilen veri:** Hata bilgileri, cihaz tipi, işletim sistemi versiyonu
- **Kişisel veri:** Gönderilmez (`sendDefaultPii: false`)
- **Gizlilik politikası:** https://sentry.io/privacy/

### 4.5 USOM (Ulusal Siber Olaylara Müdahale Merkezi)
- **Amaç:** Türkiye'ye özgü tehdit verilerinin alınması
- **İletilen veri:** Yok (yalnızca veri çekilir)
- **Kurum:** T.C. Bilgi Teknolojileri ve İletişim Kurumu

### 4.6 Diğer Tehdit İstihbarat Kaynakları
URLhaus, OpenPhish ve BOTVRIJ gibi açık kaynaklı tehdit istihbarat veritabanlarından otomatik olarak veri çekilmektedir. Bu işlemde kullanıcı verisi iletilmez.

---

## 5. Pano (Clipboard) Erişimi

SQRSeal, "Link Yakalama" özelliği etkinleştirildiğinde panonuzu periyodik olarak izler. Bu özellik:

- Yalnızca pano içeriğinin URL içerip içermediğini kontrol eder.
- URL tespit edilirse güvenlik analizi başlatır.
- URL değilse pano içeriği işlenmez ve kaydedilmez.
- Ayarlar ekranından istediğiniz zaman devre dışı bırakabilirsiniz.

---

## 6. Kamera ve Görsel Erişimi

- **QR Tarama:** Kamera yalnızca QR kod okumak için kullanılır. Görüntü kaydedilmez.
- **OCR Tarama:** Seçtiğiniz görsel, URL tespiti için geçici olarak işlenir ve analiz tamamlandıktan sonra sunucularımızdan otomatik olarak silinir.

---

## 7. Veri Saklama

| Veri | Saklama Süresi |
|------|---------------|
| Sorgu geçmişi | Siz silene kadar veya hesap silme talebine kadar |
| Teknik metrikler | 90 gün |
| Crash raporları (Sentry) | 90 gün |
| Anonim kullanım istatistikleri | Süresiz (kişiyle ilişkilendirilemez) |
| OCR görselleri | Analiz tamamlandıktan sonra anında silinir |

---

## 8. Veri Güvenliği

- Tüm iletişim HTTPS/TLS şifrelemesi ile korunur.
- API anahtarları ve hassas bilgiler yalnızca sunucu tarafında saklanır; uygulama içinde açık olarak bulunmaz.
- Veritabanı erişimi Row Level Security (RLS) politikalarıyla kısıtlanmıştır.
- Sorgu kayıtlarınıza yalnızca cihaz kimliğinizle erişilebilir.

---

## 9. Haklarınız ve Veri Silme

**Verilerinizi silme hakkına sahipsiniz.**

Uygulama içinden tüm verilerinizi silebilirsiniz:
1. Profil ekranını açın
2. Ayarlar sekmesine gidin
3. "Tüm Verilerimi Sil" butonuna tıklayın
4. Onay verdikten sonra aşağıdaki veriler kalıcı olarak silinir:
   - Tüm sorgu geçmişi
   - Kullanım istatistikleri
   - Cihaz kaydı

**Not:** Anonim teknik metrikler (yanıt süreleri, kullanım olayları), kişiyle ilişkilendirilemez oldukları için silinmeyebilir. Bu veriler yalnızca toplam istatistikler olarak analiz edilir.

KVKK kapsamındaki haklarınız için destek@sqrseal.com adresine başvurabilirsiniz.

---

## 10. Çocukların Gizliliği

SQRSeal 13 yaşın altındaki çocuklara yönelik değildir ve bilerek bu yaş grubundan veri toplamaz. Ebeveyn ya da yasal vasi olarak çocuğunuzun veri paylaştığını düşünüyorsanız lütfen bizimle iletişime geçin.

---

## 11. KVKK Uyumu

SQRSeal, 6698 sayılı Kişisel Verilerin Korunması Kanunu'na (KVKK) uygun olarak faaliyet göstermektedir.

- **Veri sorumlusu:** SQRSeal
- **İletişim:** destek@sqrseal.com
- **Web sitesi:** https://sqrseal.com

KVKK kapsamında aşağıdaki haklara sahipsiniz:
- Kişisel verilerinizin işlenip işlenmediğini öğrenme
- Kişisel verileriniz hakkında bilgi talep etme
- İşlenme amacını öğrenme
- Yurt içinde veya yurt dışında aktarıldığı üçüncü kişileri öğrenme
- Eksik veya yanlış işlenmişse düzeltme talep etme
- Silinmesini veya yok edilmesini talep etme
- Otomatik sistemler vasıtasıyla aleyhine sonuç doğurmasına itiraz etme

---

## 12. Politika Değişiklikleri

Bu politikayı güncelleme hakkımızı saklı tutarız. Önemli değişikliklerde uygulama içi bildirim yapılır. Güncel politikaya her zaman sqrseal.com/privacy adresinden ulaşabilirsiniz.

---

## 13. İletişim

Gizlilik politikamıza ilişkin sorularınız için:

**E-posta:** destek@sqrseal.com  
**Web sitesi:** https://sqrseal.com  
**Uygulama:** Profil → Ayarlar → Gizlilik Politikası

---

*SQRSeal — Dijital dünyada güvende kalın.*
