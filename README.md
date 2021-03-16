# Bulut_Sistemi

<h3>Bulut Sisteminde Ağ Güvenliği Sağlama</h3>
</h3>Ağ Güvenliği:</h3>Ağ sızması (network penetration), ve oturum kaçırma (session hijacking)
saldırıları yöntemi vardır.

Sanal ağların kandırılması: VM’lerin güvenliği için her VM'yi özel fiziksel kanalları
kullanarak ana bilgisayarına bağlamak maliyetli bir çözüm olduğundan dolayı çoğu
hipervizör, VM'leri daha doğrudan ve verimli bir şekilde iletişim kurmak için bağlamak için
sanal ağları kullanmaktadır [6]. Sisteme dahil olan kötücül bir VM, sanal ağı dinleyebilir hatta
paketleri diğer VM’lere yönlendirerek ARP kandırma yapabilmektedir. Xen gibi çoğu
sanallaştırma platformu, sanal ağları yapılandırmak için köprülü ve yönlendirilmiş olmak
üzere iki yöntem kullanmakta, fakat bu yöntemler de sanal ağın kandırılma olasılığını
artırmaktadır.
Ağ sızması (Network Penetration)
1. Kurum ve Kurum’a Ait İnternet Servisleri Hakkında Bilgi Toplama (Information
Gathering): Genellikle internete açık sunucu ve servislerin tespiti için uygulanan bu adım
yerel ağda da sunucu tespiti için uygulanabilir. Ek olarak bu adımda e-posta ve kullanıcı
hesap adları çeşitli kaynaklardan toplanabilir.
2. Sunucu ve Servis Tarama (Host and Service Scanning): Sistemlere temas edilen ilk
adım olan bu adımda canlı sunucular ve üzerlerindeki servisler çeşitli tarama yöntemleri
ile tespit edilir.
3. Ağ Haritasının Çıkarılması (Network Mapping): Bazen test öncesinde test ekibine
sağlanan bu bilgi diğer durumlarda yapılan taramalar sonucunda netleştirilmeye çalışılır.
Ağ haritası saldırı senaryolarının geliştirilmesinde ve nerelere odaklanması gerektiği
hakkında test ekibine yardımcı olabilir.
4. İşletim Sistemi Tespiti (OS Fingerprinting): Farklı işletim sistemlerinin farklı servis
türleri bulunduğundan işletimi sistemi tespiti önemli bir adımdır. Ancak pek çok durumda
kolaylıkla gerçekleştirilebilir. Bu bilgi ayrıca açıklık tespiti aşamasında da yardımcı
olabilmektedir.
5. Ağ Servisleri ve Sistem Kullanıcı Tespiti (Service and User Enumeration): Bilinen
açıklıklar belirli servisler ve bu servislerin belirli versiyonları için geçerli olduğundan hedef
sistemler üzerindeki servisler ve versiyonlarının tespiti gerekmektedir. Ayrıca pek çok
sistem öntanımlı kullanıcılarla geldiğinden bu kullanıcı hesaplarının da tespit edilmesinde 
fayda vardır. Bazen öntanımlı olmayan kullanıcı hesaplarının da uzaktan tespiti mümkün
olabilmektedir.
6. Kullanıcı Parola Tespit Saldırılarının Gerçekleştirilmesi (Password Cracking):
Öntanımlı kullanıcı hesapları için öntanımlı parolalar test edilmelidir. Diğerleri için test
süre sınırları içinde kurumun parola politikası da dikkate alınmak suretiyle sözlük
saldırıları (Dictionary Attack) gerçekleştirilebilir.
7. Tespit Edilen Servis Versiyonlarına Yönelik Açıklık Tespiti ve Açıklığın Test
Edilmesi (Vulnerability Enumeration and Exploitation): Tespit edilmiş olan servisler ve
versiyonları için bilinen açıklıklar araştırılır. Bu açıklıklar için yayınlanmış olan saldırı
yöntemleri ve istismar (Exploit) kodları denenir. Tabi bu aşama belli bir riski içerdiğinden
Pentest (Sızma Testi) angajman risk yönetim kurallarına uygun hareket edilmesi
gerekmektedir.
8. Genel Ağ Güvenliği Değerlendirmesi: Pentest (Sızma Testi) sırasında hedef ağ
hakkında çok değerli bir bakış açısı kazanılır. Ağ bölümlemesi, dışarı yönlü filtreleme,
host based firewall kurallarının kullanımı, kriptolama kullanımı, v.d. pek çok faktör Pentest
(Sızma Testi) uzmanının işini kolaylaştırır veya zorlaştırır. Bu perspektifin Pentest (Sızma
Testi) raporuna yansıtılması altyapı mimari ve BT süreçlerinin önem ve etkilerini de
somutlaştıracağından kuruma yüksek fayda sağlar.
Oturum Kaçırma(Session Hijacking)
Session hijacking, kurbanların cookie bilgilerini bir şekilde elde ederek bu cookie bilgisinin
saldırganın tarayıcısına enjekte edilmesi sonucu, kurbanın hesabına giriş yapabilmesi
olayıdır.
Kurbanın bilgisayarındaki cookie bilgilerinin çalınması için bir çok yol ve yöntem vardır,
bunlardan en çok kullanılanı, MiTM yani Man in the Middle saldırılarıdır. MiTM saldırılarına
örnek olarak Arp Poising saldırılarını örnek verebiliriz.
Nasıl Önlem Alırız
• Cookie bilginizi çaldırmamanız gerekiyor. Bunun için ARP Poisoning ve MiTM
saldırılarından tamamen korunmanız gerekmekte.
Bu saldırılardan korunabileceğiniz güvenlik uygulamalarını kullanmanızı tavsiye
ederim.
• Cookie bilginizi bulunduğunuz ağ üzerinden çaldırma ihtimaliniz çok yüksek.
Savunmasızken halka açık ağlara katılmamaya özen gösterin.
