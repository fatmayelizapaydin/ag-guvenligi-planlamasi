# Yazılım Ekibi - Güvenlik Duvarı Politikaları ve Araç Adayları

Bu doküman, Yazılım Ekibi'nin geliştirme süreçlerinde ve harici API/sunucu erişimlerinde kullandığı güvenlik duvarı entegrasyonlarını ve kriterlerini içerir.

## 1. Geliştirme Ortamı Güvenlik Kriterleri
* **Trafik Profili:** Yüksek oranda dış kaynak API istekleri, GitHub/GitLab erişimleri ve CI/CD pipeline veri akışı.
* **Özel İhtiyaçlar:** Geliştiriciler için esnek ama kontrollü port açılışları ve SSL Inspection istisnaları.

## 2. Güvenlik Duvarı ve Ağ Geçidi Adayları
1. **Fortinet FortiGate (Entegre Çözüm):** Kurumsal altyapıyla tam uyumlu olduğu için yazılım ekibi VLAN'larında da ana güvenlik katmanı olarak konumlandırılmıştır.
2. **Palo Alto Networks (DevSecOps Entegrasyonu):** API tabanlı güvenlik yönetimi için güçlü alternatifler sunar.
3. **Cisco Firepower:** Kurumsal ağ segmentasyonunda esneklik sağlar.
4. **pfSense / OPNsense (Lab ve Test Ortamları İçin):** Yazılım ekibinin kendi iç test lablarında deneme amaçlı kullandığı açık kaynaklı alternatif güvenlik duvarıdır.
5. **Check Point Next-Gen Gateway:** Gelişmiş tehdit koruması ve uygulama kontrolü amacıyla değerlendirilmiştir.
6. 
