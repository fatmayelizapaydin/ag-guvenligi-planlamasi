# Kurumsal Ağ Altyapısı ve Güvenlik Duvarı Ortak Kurulum Adımları

Bu doküman, kurumun tüm ofis ve şubelerinde standart ve güvenli bir ağ mimarisi kurmak için izlenecek temel adımları tanımlar.

## 1. Fiziksel ve Mantıksal Konumlandırma
* **Konum:** Tüm şubelerde Next-Generation Firewall (NGFW) cihazları, ana internet çıkışı (ISP) ile dahili ağ (LAN) arasına konumlandırılacaktır.
* **Yüksek Erişilebilirlik (HA):** Trafik sürekliliği ve donanım arızalarına karşı tüm şubelerde aktif-pasif veya aktif-aktif **HA (High Availability)** mimarisi zorunludur.

## 2. Ağ Segmentasyonu (VLAN Yapılandırması)
Ağ güvenliğini artırmak ve yetkisiz erişimleri önlemek amacıyla şubeler aşağıdaki mantıksal alt ağlara (VLAN) bölünecektir:
* **VLAN 10 - Yönetim (Management):** Sadece IT ve güvenlik ekiplerinin erişebileceği yönetim ağı.
* **VLAN 20 - Personel / İdari:** İdari personel ve akademisyenlerin kullandığı kurumsal ağ.
* **VLAN 30 - Öğrenci / Misafir (Guest):** Akademik şubede öğrencilerin izole şekilde internete çıkacağı kısıtlı ağ.
* **VLAN 40 - Sunucu / Ar-Ge / Yazılım:** Kritik sunucuların, test ortamlarının ve geliştirme projelerinin barındırıldığı güvenli bölge.

## 3. Temel Güvenlik İlkeleri (Security Policies)
* **Default Deny (Varsayılan Reddet):** Kurallar tablosunun en altında tüm trafik (Implicit Deny) engellenecektir.
* **IPS ve Antivirüs:** Tüm güvenlik duvarlarında IDS/IPS (Saldırı Önleme Sistemleri) ve antivirüs motorları aktif hale getirilecektir.
* 
