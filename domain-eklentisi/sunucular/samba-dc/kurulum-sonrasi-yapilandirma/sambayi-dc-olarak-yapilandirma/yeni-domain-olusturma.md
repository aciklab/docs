# Yeni Domain Oluşturma

Derlediğimiz deb paketi ile birlikte gelen yardımcı komutlar sayesinde rahatlıkla yeni bir domain kurulabilir. Deb paketi yüklendikten sonra aşağıdaki komutun çalıştırılması yeterlidir.

```text
sudo smb-create-domain -d ORNEK.LAB        
```

Domain kurulumu sırasında, Aktif Dizin'deki gibi otomatik oluşturulan Administrator kullanıcısı için parola girilmesi istenmektedir. Administrator kullanıcısı Domaindeki yetkili kullanıcı olduğundan, yetki gerektiren tüm işlemler başlangıçta bu kullanıcı ile yapılmaktadır. Bu nedenle parola bilgisi kaybedilmemelidir. 



