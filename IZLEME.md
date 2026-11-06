# Ağ ve Güvenlik Duvarı İzleme (Monitoring) Stratejisi

Bu doküman, kurumun tüm ofis ve şubelerindeki ağ trafiğinin, güvenlik duvarlarının (NGFW) ve sistem sağlığının izlenmesi için hem teknik (sistematik) hem de operasyonel (insani) süreçleri tanımlar.

## 1. Sistematik İzleme (Teknik ve Otomatik Altyapı)
Sistemlerin 7/72 kesintisiz izlenebilmesi ve anlık tehdit tespiti için şu teknik araçlar ve protokoller kullanılacaktır:
* **SIEM ve Log Yönetimi:** Tüm FortiGate güvenlik duvarlarından gelen loglar merkezi bir SIEM (Security Information and Event Management) sistemine Syslog protokolü ile aktarılacaktır.
* **SNMP ve Ağ İzleme:** Ağ cihazlarının CPU, RAM, arayüz (interface) durumları ve bant genişliği doluluk oranları SNMP v3 ve Zabbix/Grafana araçlarıyla anlık olarak izlenecektir.
* **Alert (Alarm) Mekanizmaları:** Bant genişliği %85'i geçtiğinde veya kritik bir güvenlik duvarı kuralı tetiklendiğinde IT güvenlik ekibine otomatik e-posta ve SMS uyarıları gönderilecektir.

## 2. İnsani İzleme (Operasyonel Süreçler ve İnsan Faktörü)
Profesyonel dünyada sadece yazılımlara güvenilmez; insan denetimi ve süreç yönetimi kritik rol oynar:
* **SOC (Security Operations Center) Ekibi:** 7/24 vardiyalı çalışan güvenlik analistleri, SIEM üzerine düşen anomalileri ve kritik uyarıları canlı olarak inceler.
* **Günlük Kontroller ve Raporlama:** Sabah vardiyası değişimlerinde önceki geceye ait güvenlik olayları (firewall bloklamaları, başarısız oturum açma denemeleri) manuel olarak gözden geçirilir.
* **Yetki ve Sorumluluk Matrisi (RACI):** Olay müdahale (Incident Response) süreçlerinde kimin haberdar edileceği, hangi birimin müdahale edeceği net bir şekilde tanımlanmıştır.
* 
