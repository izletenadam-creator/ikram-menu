# 🌯 İkram Çiğköfte - Akıllı Adisyon & Dijital Menü Sistemi

Bu depo, "İkram Çiğköfte" işletmesi için hazırlanan yeni nesil otonom restoran işletim sisteminin kaynak kodlarını içerir. 
Sistem sadece bir dijital menü olmakla kalmayıp, kendi kendini pazarlayan (Viral Loop) ve 2 yıllık otonom kampanya takvimini yöneten bir e-ticaret altyapısına dönüştürülmüştür.

---

## 🚀 Faz 1: Temel Sipariş Sistemi (Tamamlandı)
*   **Sepet Mantığı:** `index.html` interaktif bir alışveriş sepetine dönüştürüldü.
*   **Dinamik Fiyat & Miktar:** Toplam tutar otomatik hesaplanıp Floating Cart (Yüzen Sepet) eklendi.
*   **Adres & Konum Formu:** Modal üzerinden GPS ile otomatik konum çekme özelliği sağlandı.
*   **WhatsApp Checkout:** Siparişler anında formatlanıp `0545 442 26 26` hattına WhatsApp üzerinden aktarıldı.

---

## 🔥 Faz 2: Otonom Pazarlama & Markalaşma (Tamamlandı - 01.05.2026)
*   **Özel Domain Entegrasyonu:** İşletme resmi olarak `https://ikramciğköftesimav.com/` adresine taşındı. SEO ayarları JSON-LD ile "FastFoodRestaurant" şemasında eklendi (ChatGPT ve Gemini önerileri için hazırlandı).
*   **Otonom Kampanya Takvimi:** 2026-2027 yıllarını kapsayan, özel günleri (1 Mayıs, Bayramlar vb.) ve haftalık periyotları (Öğrenci Günleri) otomatik tanıyan fiyat kırma/indirim motoru yazıldı.
*   **Viral Döngü (Paylaş & Kazan):** Müşterilerin menüyü kendi WhatsApp'larında arkadaşlarına gönderip puan (10 Sipariş = 1 Dürüm) kazanabilecekleri **Referans Takip Sistemi** eklendi. (Referans isimleri adisyona düşer).
*   **POS Canlı Bildirim (Ntfy.sh):** Sipariş verildiği an restorandaki POS cihazına / telefona `ntfy.sh` üzerinden anlık "ZİL ÇALDIRAN" kırmızı acil bildirim entegre edildi.

---

## 🛠️ Sıradaki Adım (Faz 3 - Veritabanı ve Admin Paneli)
Sistemi manuel çentik atmadan kurtarıp tam kurumsal yapıya geçirmek için **Supabase (PostgreSQL)** mimarisi kurulacaktır.

*   **Günlük Kasa:** Hangi saatte kaç sipariş geldi, kaç TL ciro yapıldı?
*   **Otomatik Referans Sayacı:** Hangi müşteri kaç sipariş getirdi ve 10'a ulaştı mı?
*   **Stok Düşümü:** Satılan çiğköfte ve ayranın stoktan otomatik düşmesi ve bitmeye yakın kırmızı alarm vermesi.
*   **Gizli Admin Paneli (`admin.html`):** İşletme sahibinin özel bir şifreyle girip tüm bu sistemi tek ekrandan yönetebileceği merkezi kokpit.

