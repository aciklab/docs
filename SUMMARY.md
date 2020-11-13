# Table of contents

* [Liman Rehber](README.md)

## İŞLETİM SİSTEMİ KURULUMU <a id="kurulum"></a>

* [Kuruluma Giriş](kurulum/kurulum-giris.md)
* [USB ile Başlatma](kurulum/kurulum-usb/README.md)
  * [Fiziksel cihazda USB ile başlatma](kurulum/kurulum-usb/fiziksel.md)
  * [Sanal cihazda USB ile başlatma](kurulum/kurulum-usb/sanal/README.md)
    * [VirtualBox üzerinde USB başlatma](kurulum/kurulum-usb/sanal/virtualbox.md)
    * [Proxmox üzerinde USB başlatma](kurulum/kurulum-usb/sanal/proxmox.md)
* [Kurulum Süreçleri](kurulum/kurulum-surecleri/README.md)
  * [Pardus 19 Sunucu Kurulumu](kurulum/kurulum-surecleri/pardus-19-sunucu-kurulumu.md)
  * [Ubuntu 18.04 Sunucu Kurulumu](kurulum/kurulum-surecleri/ubuntu-18.04-sunucu-kurulumu.md)
* [Kurulum Sonrası Ayarlar](kurulum/kurulum-sonrasi-ayarlar.md)

## LİMAN KURULUMU

* [Liman Kurulum Yöntemleri](liman-kurulumu/liman-kurulum-yoentemleri/README.md)
  * [Paket ile Kurulum](liman-kurulumu/liman-kurulum-yoentemleri/paket-ile-kurulum.md)
  * [Depo üzerinden kurulum](liman-kurulumu/liman-kurulum-yoentemleri/depo-uezerinden-kurulum.md)
* [Liman Güncelleme](liman-kurulumu/liman-guencelleme/README.md)
  * [Paket ile Güncelleme](liman-kurulumu/liman-guencelleme/paket-ile-guencelleme.md)
  * [Depo üzerinden güncelleme](liman-kurulumu/liman-guencelleme/depo-uezerinden-guencelleme.md)
* [Kurulum Sonrası Ayarlar](liman-kurulumu/kurulum-sonrasi-ayarlar.md)
* [Liman'a Eklenti Kurulumu ve Güncellenmesi](liman-kurulumu/limana-eklenti-kurulumu.md)

## LİMAN ÜZERİNDE SUNUCU YÖNETİMİ <a id="liman-uzerinde-sunucu-yonetimi"></a>

* [Sunucu Ekleme ve Kaldırma](liman-uzerinde-sunucu-yonetimi/sunucu-ekleme.md)
* [Sunucu Ayarlarının Düzenlenmesi](liman-uzerinde-sunucu-yonetimi/sunucu-ayarlarinin-duezenlenmesi.md)
* [Sunucu'da Eklenti Kullanılması](liman-uzerinde-sunucu-yonetimi/sunucuda-eklenti-kullanilmasi.md)
* [Sunucu Yönetimi](liman-uzerinde-sunucu-yonetimi/sunucu-yonetimi.md)

## LİMAN ÜZERİNDE KULLANICI YÖNETİMİ

* [Liman Yetki Yönetimi](liman-uezerinde-kullanici-yoenetimi/liman-yetki-yonetimi/README.md)
  * [Liman Kullanıcı Ayarları](liman-uezerinde-kullanici-yoenetimi/liman-yetki-yonetimi/liman-kullanici-ayarlari.md)

## Domain Eklentisi

* [Domain Eklentisi Genel](domain-eklentisi/domain-eklentisi-genel.md)
* [Sunucular](domain-eklentisi/sunucular/README.md)
  * [SAMBA DC](domain-eklentisi/sunucular/samba-dc/README.md)
    * [Kurulum](domain-eklentisi/sunucular/samba-dc/kurulum/README.md)
      * [Paket ile Kurulum](domain-eklentisi/sunucular/samba-dc/kurulum/paket-ile-kurulum.md)
    * [Kurulum Sonrası Yapılandırma](domain-eklentisi/sunucular/samba-dc/kurulum-sonrasi-yapilandirma/README.md)
      * [Sambayı DC Olarak Yapılandırma](domain-eklentisi/sunucular/samba-dc/kurulum-sonrasi-yapilandirma/sambayi-dc-olarak-yapilandirma/README.md)
        * [Yeni Domain Oluşturma](domain-eklentisi/sunucular/samba-dc/kurulum-sonrasi-yapilandirma/sambayi-dc-olarak-yapilandirma/yeni-domain-olusturma.md)
        * [Mevcut Domaine Ekleme](domain-eklentisi/sunucular/samba-dc/kurulum-sonrasi-yapilandirma/sambayi-dc-olarak-yapilandirma/mevcut-domaine-ekleme.md)
  * [MS Aktif Dizin](domain-eklentisi/sunucular/ms-aktif-dizin/README.md)
    * [Kurulum](domain-eklentisi/sunucular/ms-aktif-dizin/kurulum.md)
* [Domain Eklentisi Arayüzü](domain-eklentisi/domain-eklentisi-arayuezue/README.md)
  * [Kullanıcı Yönetimi](domain-eklentisi/domain-eklentisi-arayuezue/kullanici-yoenetimi.md)
  * [Grup Yönetimi](domain-eklentisi/domain-eklentisi-arayuezue/grup-yoenetimi.md)
  * [Makine Yönetimi](domain-eklentisi/domain-eklentisi-arayuezue/makine-yoenetimi.md)
  * [Politika Yönetimi](domain-eklentisi/domain-eklentisi-arayuezue/politika-yoenetimi.md)

## Kaptan Servisi

* [Kaptan Servisi Hakkında](kaptan-servisi/kaptan-servisi-hakkinda.md)
* [Kaptan Kurulumu](kaptan-servisi/kaptan-kurulumu/README.md)
  * [Depodan Yükleme](kaptan-servisi/kaptan-kurulumu/depodan-yuekleme.md)
  * [Paket ile Yükleme](kaptan-servisi/kaptan-kurulumu/paket-ile-yuekleme.md)
* [Liman Kaptan Eklentisi](kaptan-servisi/liman-kaptan-eklentisi.md)

## Tayfa Servisi

* [Tayfa Servisi Hakkında](tayfa-servisi/tayfa-servisi-hakkinda.md)
* [Tayfa Kurulumu](tayfa-servisi/tayfa-kurulumu/README.md)
  * [Liman Üzerinden Palamar ile yükleme](tayfa-servisi/tayfa-kurulumu/liman-uezerinden-palamar-ile-yuekleme.md)
  * [Depodan Yükleme](tayfa-servisi/tayfa-kurulumu/depodan-yuekleme.md)
  * [Paket ile Yükleme](tayfa-servisi/tayfa-kurulumu/paket-ile-yuekleme.md)
* [Tayfa Politikaları](tayfa-servisi/tayfa-politikalari.md)

## DNS Eklentisi

* [DNS Eklentisi Genel](dns-eklentisi/dns-eklentisi-genel.md)
* [Sunucular](dns-eklentisi/sunucular.md)
* [DNS Eklentisi Arayüzü](dns-eklentisi/dns-eklentisi-arayuezue.md)

## PostgreSQL Eklentisi

* [PostgreSQL Eklentisi Genel](postgresql-eklentisi/postgresql-eklentisi-genel.md)
* [Sunucular](postgresql-eklentisi/sunucular.md)
* [PostgreSQL Eklentisi Arayüzü](postgresql-eklentisi/postgresql-eklentisi-arayuezue.md)

## Konteyner Eklentisi

* [Konteyner Eklentisi Genel](konteyner-eklentisi/konteyner-eklentisi-genel.md)
* [Sunucular](konteyner-eklentisi/sunucular.md)
* [Konteyner Eklentisi Arayüzü](konteyner-eklentisi/konteyner-eklentisi-arayuezue.md)

