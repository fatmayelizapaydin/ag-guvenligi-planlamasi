# Ar-Ge Ekibi - Kurulum Adımları ve Güvenlik Duvarı Kural Setleri

Bu doküman, Ar-Ge Ekibi'nin deneysel çalışma ve simülasyon lab ortamları için uygulanan güvenlik duvarı yapılandırma adımlarını ve kural setlerini içerir.

## 1. Ar-Ge Ekibi Kurulum Adımları
* **Deneysel Lab İzolasyonu:** Ar-Ge ekibinin üretim (production) ağlarından tamamen izole edilmiş, kendi içinde özgürce test yapabildiği sandboxing alt ağları kurulmuştur.
* **Sanal Güvenlik Duvarı (FortiGate-VM) Entegrasyonu:** Simülasyonlar ve prototip testleri için sanal güvenlik duvarı bileşenleri devreye alınmıştır.
* **Özel Trafik ve Protokol Tanımlamaları:** Araştırma projeleri kapsamında kullanılan standart dışı network protokolleri için özel güvenlik duvarı istisnaları tanımlanmıştır.

## 2. Ar-Ge Ekibi Güvenlik Duvarı Kural Setleri (Policy Rules)
* **Kural 1 (Sandbox Lab Erişimi):** Ar-Ge laboratuvarındaki test sunucularının dış dünya ile kontrollü ve güvenli veri alışverişi kuralı.
* **Kural 2 (Simülasyon Trafik Kısıtlaması):** Deneysel ağ trafiğinin ana kurumsal omurgayı etkilememesi için bant genişliği önceliklendirme ve yönlendirme kuralları.
* **Kural 3 (Default Deny):** Güvenlik politikaları gereği tanımlı kurallar dışında kalan tüm port ve IP'lere erişim varsayılan olarak engellenmiştir.
* 
