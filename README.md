# 🍔 İkram Çiğköfte - Akıllı Adisyon & Dijital Menü Sistemi

Bu depo, "İkram Çiğköfte" işletmesi için hazırlanan yeni nesil QR kodlu sipariş ve adisyon sisteminin kaynak kodlarını içerir. 
Sistem, klasik bir Yemeksepeti / Getir arayüzünün konforunu sunarken, siparişleri komisyonsuz şekilde doğrudan işletmenin WhatsApp hattına ve yerel bot/dashboard ekranına iletmek üzere tasarlanmaktadır.

## 🚀 Faz 1: Web Sitesinin Dinamikleşmesi (Tamamlandı - 30.04.2026)
*   **Sepet Mantığı:** `index.html` içindeki statik menü, JavaScript kullanılarak interaktif bir alışveriş sepetine dönüştürüldü.
*   **Miktar Kontrolleri:** Her ürünün yanına `[ - ] 0 [ + ]` butonları eklendi.
*   **Dinamik Fiyat Hesaplama:** Sepete eklenen ürünlere göre toplam tutar otomatik hesaplanıp alttaki *Floating Cart (Yüzen Sepet)* çubuğuna yansıtıldı.
*   **Adres & Konum Formu:** Siparişi Tamamla butonuna basıldığında açılan şık bir Modal/Popup tasarlandı.
*   **GPS Entegrasyonu:** HTML5 Geolocation API kullanılarak tek tuşla kullanıcının GPS konumunun adrese otomatik yazılması sağlandı.
*   **WhatsApp Checkout:** Girilen isim, adres ve sepetteki ürünler formatlı bir fiş/adisyon metnine dönüştürülüp, doğrudan `0545 442 26 26` WhatsApp hattına yönlendirme sağlandı.

## 🛠️ Sıradaki Adım (Faz 2)
*   Siteden sipariş verildiğinde, JavaScript `fetch` API ile yerel sunucumuzdaki (instagram-bot altındaki) Python botuna HTTP POST isteği gönderilerek dükkandaki bilgisayarda sesli "Yeni Sipariş" alarmı oluşturulacak.
