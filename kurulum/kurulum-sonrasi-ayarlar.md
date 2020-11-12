# Kurulum Sonrası Ayarlar

İşletim sistemini kurduktan sonra en önemli ayarlardan birisi sistemin güncel olup olmamasıdır. Bu hem güvenlik nedeni ile hem de güncel sistem araçlarının kullanılması ihtiyaçları nedeniyle önemli bir davranıştır.

## 1. Sistemin güncelliğinin kontrol edilmesi

Sistemin güncelliğini kontrol edilmesi için Debian tabanlı tüm sistemlerde aşağıdaki komut uygulanır.

```text
sudo apt update
```

Bu komut ile birlikte sisteminizde güncellenme ihtiyacı bulunan paket olup olmadığı gösterilmektedir. Fakat herhangi bir güncelleme işlemi yapmaz. İlgili paketleri güncellemek istediğinizde ise aşağıdaki komut uygulanır.

```text
sudo apt upgrade
```

Bu işlem tamamlandığında herhangi bir problem yoksa sisteminiz güncellenmiş olacaktır.

## 2. Statik IP ayarlanması

Pardus ve Ubuntu kurulumunda eğer Elle IP ayarı girmediyseniz varsayılan olarak sisteminizde DHCP varsa, ilgili sunucu tarafından size bir IP atanacaktır. Fakat bu IP adresi belirli kurallarla belirli zaman sonra değişebilir. Bu nedenle bunu sabit hale getirmek için sistem üzerinden sabit IP tanımlamanız gerekmektedir.

## 2.1. Pardus Sunucu üzerinde statik IP verme

Hem Pardus 17.x hem de Pardus 19.x sürümlerinde statik IP verme süreci aynıdır. Bu nedenle **/etc/network/interfaces** dosyası içerisine girilir. Bu dosya içerisinde aşağıdaki gibi bir satır bulunması gerekir.

```text
iface eth0 inet dhcp
```

Bu ve benzeri yapıda anlatılan şey **eth0** ağ arabiriminde **DHCP** ile otomatik IP alınmasıdır. Dolayısıyla bu dosyadaki tek satırı yönetici yetkili bir hesap ile vim veya nano gibi bir araç ile açıp, aşağıdaki gibi değiştirmeniz gerekmektedir:

```text
iface eth0 inet static
      address 192.168.1.67
      netmask 255.255.255.0
      gateway 192.168.1.1
```

Bu kod dizisindeki IP adresi olarak belirtilen 192.168.1.67 IP'si yerine sizin daha önce aldığınız ip adresini yazabilirsiniz. Bunun için dosyayı düzenlemeye başlamadan "ip a" komutu ile DHCP'nin size verdiği IP adresini öğrenip onu yazabilirsiniz. Gateway ve DNS adresleri eklenmesi gerekiyorsa bu konuda daha detaylı içeriği internetteki detaylı kaynaklardan bulabilirsiniz.

## 2.2. Ubuntu Sunucu üzerinde statik IP verme

Ubuntu, 18.04 sürümünden sonra klasik ağ yapısı yerine netplan sistemine geçmiştir. İlk olarak ağ arabirimi ve mevcut IP'nin belirlenmesi için "ip a" komutunu uygulayarak eth0 veya ens0s3 gibi değer belirlenir.

Bu adımdan sonra **/etc/netplan/01-netcfg.yaml** dosyası içerisine girilir. Bu dosya içerisinde aşağıdaki gibi bir görüntü bulunmaktadır:

```text
network:
  version: 2
  renderer: networkd
  ethernets:
    ens0s3:
      dhcp4: yes
```

Bu içerik, aşağıdaki gibi bir hale getirilir:

```text
network:
  version: 2
  renderer: networkd
  ethernets:
    ens0s3:
      dhcp4: no
      addresses:
        - 192.168.1.67/24
      gateway4: 192.168.1.1
      nameservers:
          addresses: [8.8.8.8]
```

Yaml dosyası olduğu için boşluklar önemlidir. Ve bu düzenleme yapıldıktan sonra aşağıdaki komut ile netplan uygulanmış olur:

```text
sudo netplan apply
```

Böylelikle IP adresi alınmış olur. Daha detaylı bilgi için internette çok daha detaylı bilgilere erişebilirsiniz.

