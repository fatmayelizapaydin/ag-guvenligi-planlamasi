# Yazılım Ekibi - Kurulum Adımları ve Güvenlik Duvarı Kural Setleri

Bu doküman, Yazılım Ekibi'nin geliştirme ve test ortamları için uygulanan güvenlik duvarı yapılandırma adımlarını ve kural setlerini içerir.

## 1. Yazılım Ekibi Kurulum Adımları
* **Ağ Segmentasyonu:** Geliştiricilerin bağlı olduğu VLAN üzerinde diğer idari ağlardan izole edilmiş özel bir alt ağ tanımlanmıştır.
* **Güvenli Tünel (VPN) Yapılandırması:** Uzaktan çalışan yazılımcıların sisteme güvenli erişimi için SSL-VPN ve iki aşamalı doğrulama (MFA) entegrasyonu tamamlanmıştır.
* **İstisna ve Port Tanımlamaları:** CI/CD süreçleri ve dış API testleri için gerekli giden port (egress) izinleri güvenlik duvarı üzerinde tanımlanmıştır.

## 2. Yazılım Ekibi Güvenlik Duvarı Kural Setleri (Policy Rules)
* **Kural 1 (Geliştirici Internet Erişimi):** Geliştiricilerin kod tabanlarına (GitHub, GitLab vb.) ve paket yöneticilerine güvenli erişimi için özel kural tanımlanmıştır.
* **Kural 2 (Test Ortamı İzolasyonu):** Test (Stage) sunucularına sadece yetkili yazılım personelinin erişebileceği kaynak IP kısıtlamaları getirilmiştir.
* **Kural 3 (Default Deny):** Güvenlik politikaları gereği tanımlı kurallar dışında kalan tüm port ve IP'lere erişim varsayılan olarak engellenmiştir.
* 
