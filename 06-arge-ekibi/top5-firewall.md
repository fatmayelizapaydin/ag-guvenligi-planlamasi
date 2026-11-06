# Ar-Ge Ekibi - Güvenlik Duvarı Politikaları ve Araç Adayları

Bu doküman, Ar-Ge Ekibi'nin deneysel çalışmalarında ve simülasyon ortamlarında kullandığı güvenlik duvarı entegrasyonlarını ve kriterlerini içerir.

## 1. Ar-Ge Ortamı Güvenlik Kriterleri
* **Trafik Profili:** Yüksek veri akışı, özel protokol testleri ve simülasyon trafiği.
* **Özel İhtiyaçlar:** Sandboxing (güvenli alan) teknolojileri, özel kural istisnaları ve derinlemesine paket analizi (DPI) esnekliği.

## 2. Güvenlik Duvarı ve Ağ Geçidi Adayları
1. **Fortinet FortiGate (Entegre Çözüm):** Ar-Ge laboratuvarlarında sanal firewall (FortiGate-VM) olarak konumlandırılan ve esnek test imkanı sunan birincil çözümdür.
2. **Palo Alto Networks (Gelişmiş Threat Intel):** Tehdit istihbaratı ve zararlı yazılım analizi için ar-ge ekibinin incelediği alternatif sistemdir.
3. **OPNsense / pfSense:** Ar-Ge ekibinin kendi iç ağlarında test, prototip ve sızma testleri amacıyla kullandığı açık kaynaklı güvenlik duvarıdır.
4. **Cisco Firepower:** Kurumsal omurga entegrasyonu için alternatif mimari olarak değerlendirilmiştir.
5. **Check Point SandBlast Gateway:** Sıfır gün (zero-day) saldırı analizi ve zararlı yazılım tespiti için referans alınan sistemdir.
6. 
