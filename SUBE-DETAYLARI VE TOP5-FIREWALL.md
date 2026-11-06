# Şube Bazlı Detaylı Altyapı, Bant Genişliği ve Top 5 Firewall Raporu

Bu doküman; İstanbul, Ankara, Londra ofisleri ile Akademik Şube, Yazılım ve Ar-Ge birimlerinin kişi sayılarına göre bant genişliği tahminlerini, top 5 güvenlik duvarı önerilerini ve şube özelindeki kural setlerini içerir.

## 1. Ankara Ofisi (220 Çalışan)
* **Bant Genişliği İhtiyacı:** 1.50 Gbps (2 + 1 Gbps Hat)
* **Top 5 Firewall Adayları:** 
  1. Fortinet FortiGate 200F (Seçilen Model - Optimum Fiyat/Performans)
  2. Palo Alto Networks PA-3220
  3. Cisco Firepower 2130
  4. Check Point Security Gateway 1550
  5. SonicWall NSA 6700
* **Kural Setleri:** İdari ve teknik personel için Web Filtering aktif, yönetim ağına sadece içeriden yetkili erişim, varsayılan olarak her şeyin engellenmesi (Default Deny).

## 2. İstanbul Ofisi (420 Çalışan)
* **Bant Genişliği İhtiyacı:** 3.95 Gbps (5 + 5 Gbps Hat)
* **Top 5 Firewall Adayları:**
  1. Fortinet FortiGate 400F (Seçilen Model - Yüksek UTM Kapasitesi)
  2. Palo Alto Networks PA-5220
  3. Cisco Firepower 4110
  4. Check Point Security Gateway 3200
  5. Juniper SRX 4600
* **Kural Setleri:** Yoğun kurumsal trafik için SSL Inspection ve Application Control kuralları aktif edilmiştir.

## 3. Londra Ofisi (210 Çalışan)
* **Bant Genişliği İhtiyacı:** 1.35 Gbps (2 + 1 Gbps Hat)
* **Top 5 Firewall Adayları:**
  1. Fortinet FortiGate 200F (Seçilen Model)
  2. Palo Alto Networks PA-3220
  3. Cisco Firepower 2130
  4. Check Point Security Gateway 1550
  5. SonicWall NSA 6700
* **Kural Setleri:** Uluslararası koordinasyon ve güvenli VPN tünelleri için özel kural setleri.

## 4. Akademik Şube (10,750 Kullanıcı - 10,000 Öğrenci)
* **Bant Genişliği İhtiyacı:** 27.09 Gbps (30 + 10 Gbps Hat)
* **Top 5 Firewall Adayları:**
  1. Fortinet FortiGate 3500F (Seçilen Model - Çok Yüksek Throughput)
  2. Palo Alto Networks PA-7050
  3. Cisco Firepower 9300
  4. Check Point 65000 Security System
  5. Juniper SRX 5800
* **Kural Setleri:** Öğrenci VLAN'larında Rate Limiting (Bant Genişliği Sınırlaması) ve P2P/Torrent trafik engelleme kuralları.
* 
