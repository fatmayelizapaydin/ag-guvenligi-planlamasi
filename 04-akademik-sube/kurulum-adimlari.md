# Akademik Şube - Kurulum Adımları ve Güvenlik Duvarı Kural Setleri

Bu doküman, Akademik Şube'ye özel FortiGate 3500F güvenlik duvarının kurulum aşamalarını, test süreçlerini ve kampüs geneli kural setlerini tanımlar.

## 1. Akademik Şube Kurulum Adımları
* **Yüksek Kapasiteli Arayüz Yapılandırması:** 30 Gbps ana hat ve 10 Gbps yedek hat için 100G/40G fiber portlar ve LACP (Link Aggregation) yapılandırması tamamlanmıştır.
* **HA ve Yedekleme Mimarisi:** Devasa kampüs trafiğinin kesintiye uğramaması için FortiGate 3500F cihazları yüksek kullanılabilirlik (HA) modunda yapılandırılmıştır.
* **VLAN ve Alt Ağ Segmentasyonu:** Öğrenci laboratuvarları, derslikler, kampüs Wi-Fi ağları ve idari birimler için ayrı VLAN ve alt ağlar tanımlanmıştır.

## 2. Akademik Şube Güvenlik Duvarı Kural Setleri (Policy Rules)
* **Kural 1 (Öğrenci Ağları Sınırlaması):** Öğrenci VLAN'larında bant genişliği tüketimini dengelemek için Rate Limiting ve P2P/Torrent trafik engelleme kuralları aktif edilmiştir.
* **Kural 2 (Akademik Erişim ve Web Filtreleme):** Eğitim portallarına ve akademik kaynaklara kesintisiz erişim sağlanırken, zararlı ve uygunsuz siteler için Web Filtering uygulanmaktadır.
* **Kural 3 (Default Deny):** Kampüs ağ güvenliğini en üst düzeyde tutmak amacıyla tanımlı kurallar dışındaki tüm yetkisiz erişimler varsayılan olarak engellenmiştir.
* 
