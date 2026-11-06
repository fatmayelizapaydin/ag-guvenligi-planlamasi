# İstanbul Ofisi - Kurulum Adımları ve Güvenlik Duvarı Kural Setleri

Bu doküman, İstanbul Ofisi'ne özel FortiGate 400F güvenlik duvarının kurulum aşamalarını, test süreçlerini ve yerel kural setlerini tanımlar.

## 1. İstanbul Ofisi Kurulum Adımları
* **Arayüz (Interface) Yapılandırması:** WAN1 ve WAN2 portlarına toplam 10 Gbps (5 + 5 Gbps) kapasiteli ana ve yedek ISP hatları yük dengeleme (Load Balancing) ile tanımlanmıştır.
* **HA (High Availability) Yapılandırması:** Merkez ofis sürekliliği için FortiGate 400F cihazları aktif-pasif HA mimarisiyle yapılandırılmıştır.
* **VLAN ve Switch Entegrasyonu:** İdari, yazılım, teknik, ar-ge ve güvenlik birimleri için ayrı ayrı VLAN segmentasyonları tamamlanmıştır.

## 2. İstanbul Ofisi Güvenlik Duvarı Kural Setleri (Policy Rules)
* **Kural 1 (Kurumsal Internet Erişimi):** Personel VLAN'larından gelen HTTP/HTTPS trafiği için SSL Inspection, Deep Packet Inspection (DPI) ve Web Filtering kuralları uygulanır.
* **Kural 2 (Sunucu ve Ar-Ge Erişimi):** Ar-Ge ve yazılım ekiplerinin dış dünya ile güvenli tünel (IPsec VPN) bağlantıları tanımlanmıştır.
* **Kural 3 (Default Deny):** Güvenlik politikaları gereği tanımlı kurallar dışında kalan tüm port ve IP'lere erişim varsayılan olarak engellenmiştir.
* 
