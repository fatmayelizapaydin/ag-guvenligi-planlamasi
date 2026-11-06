# Ağ Güvenliği ve Firewall - Test ve Kullanım Senaryoları

Bu doküman, projede yer alan tüm şube ve birimler (Ankara, İstanbul, Londra, Akademik Şube, Yazılım Ekip ve Ar-Ge) için oluşturulan güvenlik duvarı kurallarının doğrulanması amacıyla hazırlanan test senaryolarını içerir.

## 1. Senaryo 1: Standart Kullanıcı İnternet Erişimi ve Web Filtreleme Testi
* **Amaç:** Personel ve öğrenci VLAN'larından çıkan web trafiğinin kurallara uygun filtrelendiğini doğrulamak.
* **Test Adımları:**
  1. Personel ağındaki bir bilgisayardan zararlı yazılım içeren veya yasaklı kategorideki (örneğin bahis/kumar) bir web sitesine erişim denemesi yapılır.
  2. Güvenlik duvarının (FortiGate) Web Filtering motorunun sayfayı doğrudan bloklayıp bloklamadığı kontrol edilir.
  3. Log kayıtlarında `Deny` (Engellendi) statüsünün düşüp düşmediği incelenir.
* **Beklenen Sonuç:** Trafik güvenlik duvarı tarafından engellenmeli ve kullanıcıya uyarı sayfası gösterilmelidir.

## 2. Senaryo 2: Şubeler Arası Güvenli Tünel (IPsec VPN) Testi
* **Amaç:** Merkez (İstanbul) ile şubeler (Ankara, Londra) arasındaki haberleşmenin şifreli tüneller üzerinden yapıldığını test etmek.
* **Test Adımları:**
  1. Ankara Ofisi'ndeki bir sunucudan İstanbul Ofisi'ndeki veri tabanı sunucusuna `ping` veya `traceroute` atılır.
  2. Trafiğin açık internet üzerinden değil, kurulan IPsec VPN tüneli üzerinden geçtiği doğrulanır.
* **Beklenen Sonuç:** Paketler şifreli tünel üzerinden kayıpsız ve güvenli bir şekilde iletilmelidir.

## 3. Senaryo 3: Ar-Ge ve Yazılım Lab İzolasyonu (Sandboxing) Testi
* **Amaç:** Ar-Ge ve Yazılım ekibi laboratuvar ağlarının, kurumsal ana ağdan tamamen izole olup olmadığını denetlemek.
* **Test Adımları:**
  1. Ar-Ge test ortamından idari birimlerin yerel dosya paylaşım sunucularına erişim denenir.
  2. Güvenlik duvarının `Default Deny` kuralının bu geçişi engellediği kontrol edilir.
* **Beklenen Sonuç:** İzin verilmeyen hiçbir çapraz geçişe (lab -> idari ağ) izin verilmemelidir.

## 4. Senaryo 4: Akademik Şube Bant Genişliği ve Rate Limiting Testi
* **Amaç:** 10.000+ kullanıcılı akademik kampta yoğun ağ kullanımının (P2P/Torrent vb.) omurgayı kitlemesini engellemek.
* **Test Adımları:**
  1. Öğrenci VLAN'ından yüksek bant genişliği tüketecek indirme testleri simüle edilir.
  2. Güvenlik duvarı üzerindeki trafik şekillendirme (Traffic Shaping / Rate Limiting) kurallarının devreye girip girmediği gözlemlenir.
* **Beklenen Sonuç:** Kritik akademik sistemlerin hızı düşmeden, öğrenci ağındaki aşırı yükler otomatik olarak limitlenmelidir.
* 
