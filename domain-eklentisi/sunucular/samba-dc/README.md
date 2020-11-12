# SAMBA DC

## Samba Sunucusu Hakkında

Kurumsal sistemler için Aktif Dizin yerine ya da Aktid Dizin yanına konumlandırılabilecek açık kaynak kodlu bir uygulamadır . Samba, MS Aktif Dizin'in 2008 sürümünden yola çıkılarak geliştirilmiş. Samba 4 sürümü ile birlikte Etki Alanı Denetleyicisi özelliği de gelen Samba, MS Aktif Dizin şemaları ile aynı şemaya sahip olmasından dolayı Windows cihazları da kendi etki alanına dahil olmasına imkan vermektedir. Bunun yanı sıra MS Aktif Dizin ile tümleşik yapılar da oluşturulabilmektedir. 2008, 2008R2 şemalarının yanı sıra yakın zamandaki gelişme ile 2012 ve 2012R2 şemalarını da destekler hale gelmiştir. Ne yazıkki Aktif Dizin 2016 ve sonrası şemalarının lisanslı olmasından dolayı samba tarafından resmi destek verilmemektedir. Sambanın kendi yönetim arayüzü bulunmamaktadir. Linux üzerine kurulan samba terminal arayüzünden yönetilmektedir.

**Samba ile ne yapılabilir:**

Öncelikle Samba ile GNU/Linux sistem üzerinde klasik şekilde dosya paylaşımı oluşturup, SMB standartı ile hibrit işletim sistemlerinden erişim sağlayabilirsiniz.

GNU/Linux sistem üzerinde gerekli ayarları yaparsanız Windows Aktif Dizin gibi bir Etki Alanı Kontrolcüsü oluşturabilirsiniz.

Mevcut güncel sürümünde **Windows 2012R2 Fonksiyon seviyesi**, şema seviyesi ve orman seviyelerinde bulunan Windows Aktif Dizin Etki Alanı sistemleriyle hibrit bir şekilde güven ilişkisi kurup, çeşitli site yapılarında birlikte kullanabilirsiniz.

Kendi içerisinde bulunan **DNS** sunucususunu veya aynı sistem üzerine kuracağınız **BIND DNS** sunucusunu bağlayarak etki alanı yapınız için DNS ihtiyacınızı çözebilirsiniz.

**GPO** yapınızı olduğu gibi kullanabilirsiniz. Bu sayede etki alanında bulunan Windows makinelere yine aynı şekilde SYSVOL klasöründe bulunan politikalar ile organizasyon birimine göre kullanıcı ve makineye göre ayrı ayrı politika atayabiliyorsunuz. Mevcut yapı üzerinde GNU/Linux sistemler için bir politika altyapısı bulunmamaktadır. Fakat bizim ekibimizce geliştirdiğimiz "Liman-Kaptan-Tayfa" altyapısı ile etki alanı kontrolcüsünü kullanarak politika altyapısı sağlamaktayız.

**SAMBA güncel sürümleri:**

Samba geliştiricileri 3 Mart 2020 yılında güncel olarak 4.12.0 sürümünü duyurdular. 4.11.x serisi ise 10 Mart 2020 tarihinde 4.11.7 sürümüne ulaştı.

| İşetim Sistemi | Versiyon |  |
| :--- | :--- | :--- |
| **Centos** |  |  |
| Centos 7 | samba-4.9.1-6.el7 |  |
| Centos 8 | samba-4.10.4-101.el8\_1 | BaseOS Deposu |
|  | samba-4.9.1-8.el8 |  |
| **Debian** |  |  |
| Debian 10 | samba-4.9.5+dfsg-5+deb10u1 | kararlı |
| Debian 11 | samba-4.11.5+dfsg-1 | testing |
| Debian Sid | samba-4.11.5+dfsg-1+b1 | kararsız |
| **Ubuntu** |  |  |
| Ubuntu 18.04 | samba-4.7.6+dfsg~ubuntu-0ubuntu2.15 |  |
| Ubuntu 20.04 | samba-4.11.6+dfsg-0ubuntu1 |  |
| **Fedora** |  |  |
| Fedora 30 | samba-4.10.2-0.fc30 |  |
| Fedora 31 | samba-4.11.0-3.fc31 |  |
| Fedora Rawhide | samba-4.12.0-5.fc33.1 |  |

SAMBA'nın güncel sürümleri, [topluluğun duyuru mail listesi](https://lists.samba.org/mailman/listinfo/samba-announce) üzerinden duyurulmaktadır. Genellikle 6 ayda bir duyurulan ara sürümler sonrasında güvenlik ve bugfix güncellemeleri duyurulmaktadır. Genellikle 6 ayda bir duyurulan ara sürümler sonrasında güvenlik ve bugfix güncellemeleri duyurulmaktadır.

Samba'nın kaynak koduna [orjinal git sayfaları](https://git.samba.org/samba.git/)ndan erişilebileceği gibi, aynaladıkları [Gitlab](https://gitlab.com/samba-team/samba) üzerinden ya da [Github](https://github.com/samba-team/samba) üzerinden erişilebilir.

