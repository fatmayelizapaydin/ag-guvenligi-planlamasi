# Ankara Ofisi - Kurulum Adımları ve Güvenlik Duvarı Kural Setleri

Bu doküman, Ankara Ofisi'ne özel FortiGate 200F güvenlik duvarının kurulum aşamalarını, test süreçlerini ve yerel kural setlerini tanımlar.

## 1. Ankara Ofisi Kurulum Adımları
* **Arayüz (Interface) Yapılandırması:** WAN1 portuna 2 Gbps ana ISP hattı, WAN2 portuna 1 Gbps yedek hat tanımlanmıştır. Internal portlar yerel switch omurgasına bağlanmıştır.
* **HA (High Availability) Yapılandırması:** İki adet FortiGate 200F cihazı arasında kesintisiz operasyon için A-P (Active-Passive) HA cluster kurulumu tamamlanmıştır[span_2](start_span)[span_2](end_span).
* **DHCP ve VLAN Atamaları:** İdari personel, yazılımcı ve teknik ekipler için ilgili VLAN segmentleri aktif hale getirilmiştir.

## 2. Ankara Ofisi Güvenlik Duvarı Kural Setleri (Policy Rules)
* **Kural 1 (İçeriden Dışarıya - Internet Access):** Personel VLAN'larından WAN bacaklarına çıkan HTTP/HTTPS trafiğine Web Filtering ve Application Control uygulanır.
* **Kural 2 (Yönetim Erişimi):** Sadece güvenli yönetim VLAN'ından firewall arayüzlerine HTTPS ve SSH üzerinden erişime izin verilir.
* **Kural 3 (Default Deny):** Yukarıdaki kuralların dışındaki tüm yetkisiz ve korsan trafik varsayılan olarak engellenir (Implicit Deny).
* 
