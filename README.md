# Kurumsal Ağ Güvenliği ve Altyapı Planlaması Projesi

Bu proje; çokuluslu ve akademik operasyonlar yürüten hayali bir kurumun ağ güvenliği mimarisini, bant genişliği kapasite planlamasını ve Yeni Nesil Güvenlik Duvarı (NGFW) entegrasyonunu standartlaştırmak amacıyla tasarlanmıştır[span_0](start_span)[span_0](end_span). Kurum; İstanbul, Ankara ve Londra ofisleri ile yüksek trafikli bir Akademik Şube, Yazılım Ekibi ve Ar-Ge biriminden oluşmaktadır[span_1](start_span)[span_1](end_span)[span_2](start_span)[span_2](end_span)[span_3](start_span)[span_3](end_span).

## Proje Kapsamı ve Matris Tablosu
Her şubenin kullanıcı profili analiz edilerek hesaplanan bant genişliği gereksinimleri ve seçilen Yüksek Erişilebilirlik (HA) mimarisine sahip FortiGate NGFW modelleri aşağıda yer almaktadır[span_4](start_span)[span_4](end_span):

| Branch (Şube) | Admin Staff | Faculty | Students | Software | Technical | Security | R&D | Total (Toplam) | Required Bandwidth | Primary + Backup Link | Selected NGFW (HA) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Istanbul Office** | 280 | 0 | 0 | 60 | 35 | 25 | 20 | 420 | 3.95 Gbps[span_5](start_span)[span_5](end_span) | 5 + 5 Gbps[span_6](start_span)[span_6](end_span) | FortiGate 400F[span_7](start_span)[span_7](end_span) |
| **Ankara Office** | 140 | 0 | 0 | 30 | 20 | 15 | 15 | 220 | 1.50 Gbps[span_8](start_span)[span_8](end_span) | 2 + 1 Gbps[span_9](start_span)[span_9](end_span) | FortiGate 200F[span_10](start_span)[span_10](end_span) |
| **London Office** | 125 | 0 | 0 | 30 | 18 | 16 | 12 | 210 | 1.35 Gbps[span_11](start_span)[span_11](end_span) | 2 + 1 Gbps[span_12](start_span)[span_12](end_span) | FortiGate 200F[span_13](start_span)[span_13](end_span) |
| **Academic Branch** | 220 | 400 | 10,000 | 30 | 60 | 0 | 40 | 10,750 | 27.09 Gbps[span_14](start_span)[span_14](end_span) | 30 + 10 Gbps[span_15](start_span)[span_15](end_span) | FortiGate 3500F[span_16](start_span)[span_16](end_span) |
| **Total (Toplam)** | **775** | **400** | **10,000** | **150** | **133** | **55** | **67** | **11,600** | **34.00 Gbps**[span_17](start_span)[span_17](end_span) | **39 + 17 Gbps**[span_18](start_span)[span_18](end_span) | - |
