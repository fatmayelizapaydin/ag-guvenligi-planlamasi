# Yazılım Ekibi - Departman Analizi ve Kaynak Planlaması

Bu doküman, Yazılım Ekibi'nin geliştirme ortamı, sunucu erişimleri ve özel güvenlik gereksinimlerini içerir.

## 1. Departman Kapsamı ve Ekip Yapısı
* **Yazılım Geliştiriciler (Developers):** 45
* **DevOps ve Sistem Uzmanları:** 12
* **QA / Test Mühendisleri:** 15
* **Toplam Ekip Mevcudu:** 72

## 2. Ağ ve Güvenlik Gereksinimleri
* **Özel Segmentasyon:** Geliştirme (Dev), Test (Stage) ve Canlı (Production) ortamlar için izole VLAN yapılandırmaları.
* **Erişim Kontrolleri:** Kod repolarına ve CI/CD pipeline sunucularına sadece güvenli VPN ve MFA (Çok Faktörlü Kimlik Doğrulama) ile erişim.
* 
