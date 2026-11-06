# Londra Ofisi - Kurulum Adımları ve Güvenlik Duvarı Kural Setleri

Bu doküman, Londra Ofisi'ne özel FortiGate 200F güvenlik duvarının kurulum aşamalarını, test süreçlerini ve yerel kural setlerini tanımlar.

## 1. Londra Ofisi Kurulum Adımları
* **Arayüz (Interface) Yapılandırması:** WAN1 portuna 2 Gbps ana ISP hattı, WAN2 portuna ise 1 Gbps yedek hat tanımlanmıştır.
* **HA (High Availability) Yapılandırması:** Kesintisiz erişim için iki adet FortiGate 200F cihazı aktif-pasif modda cluster yapılmıştır.
* **VLAN Yapılandırması:** Ofis içi idari, yazılım ve teknik birimler için izole yerel ağ segmentleri oluşturulmuştur.

## 2. Londra Ofisi Güvenlik Duvarı Kural Setleri (Policy Rules)
* **Kural 1 (Internet Erişimi):** Personel VLAN'larından gelen web trafiği için Web Filtering ve Application Control aktif edilmiştir.
* **Kural 2 (Şubeler Arası VPN):** Merkez ofis ve diğer şubelerle güvenli tünel (IPsec VPN) iletişimi sağlanmıştır.
* **Kural 3 (Default Deny):** Tanımlı kurallar haricindeki tüm yetkisiz erişim denemeleri varsayılan olarak engellenir.
* 
