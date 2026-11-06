# Kurumsal Ağ Güvenliği Risk Analizi ve Tehdit Yönetimi

Bu doküman, kurumun tüm ofislerinde ve şubelerinde karşılaşılması muhtemel siber güvenlik risklerini, ağ kesintisi tehditlerini ve bunlara karşı alınacak proaktif önlemleri tanımlar.

## 1. Olası Riskler ve Tehdit Senaryoları
* **Bant Genişliği Darboğazı (Bottleneck):** Özellikle Akademik Şube'deki 10.000 öğrencinin[span_3](start_span)[span_3](end_span) yoğun internet kullanımı sırasında hatların doygunluğa ulaşması ve kritik iş süreçlerinin yavaşlaması.
* **Yetkisiz Erişim ve İç Tehditler (Insider Threats):** Personel veya öğrenci VLAN'larından yönetim ağına (Management) sızma denemeleri.
* **Donanım Arızası ve Kesinti:** Güvenlik duvarı (NGFW) cihazlarında yaşanabilecek ani donanım arızalarında tüm şube trafiğinin kesilmesi riski.
* **DDoS ve Botnet Saldırıları:** Kurumun dış dünya ile olan ana hatlarına gelebilecek hacimsel saldırılar.

## 2. Proaktif Korunma ve Mitigasyon Stratejileri
* **Yüksek Erişilebilirlik (HA):** Tüm şubelerde ana ve yedek hatlar ile HA mimarisine sahip FortiGate cihazları kullanılarak kesinti riski minimuma indirilecektir[span_4](start_span)[span_4](end_span).
* **Katı Ağ Segmentasyonu:** VLAN yapılandırmaları sayesinde kullanıcılar ile kritik sunucular tamamen izole edilecektir.
* **Trafik Şekillendirme (Traffic Shaping):** Akademik şubede öğrenci ağındaki p2p ve video akış trafiğine bant genişliği sınırlamaları (Rate Limiting) uygulanacaktır.
* 
