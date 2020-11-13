# Yeni Domain Oluşturma

Derlediğimiz deb paketi ile birlikte gelen yardımcı komutlar sayesinde rahatlıkla yeni bir domain kurulabilir. Deb paketi yüklendikten sonra aşağıdaki komutun çalıştırılması yeterlidir. **ORNEK.LAB** yerine kendi domaininizi yazabilirsiniz.

```text
sysadmin@ub18samba:~$ sudo smb-create-domain -d ORNEK.LAB
[sudo] password for sysadmin: 
Administrator parolası: 
INFO 2020-11-13 06:09:10,812 pid:6414 /opt/samba4/lib/python3.6/site-packages/samba/provision/__init__.py #2128: Looking up IPv4 addresses
INFO 2020-11-13 06:09:10,813 pid:6414 /opt/samba4/lib/python3.6/site-packages/samba/provision/__init__.py #2145: Looking up IPv6 addresses      
...
```

Domain kurulumu sırasında, Aktif Dizin'deki gibi otomatik oluşturulan Administrator kullanıcısı için parola istenmektedir. 

{% hint style="info" %}
Administrator kullanıcısı Domaindeki yetkili kullanıcı olduğundan, yetki gerektiren tüm işlemler başlangıçta bu kullanıcı ile yapılmaktadır. Bu nedenle parola bilgisi kaybedilmemelidir. 
{% endhint %}

Kurulum başarılı bir şekilde tamamlandı ise, aşağıdaki gibi INFO formatında domain bilgileri, self-signed sertifika oluşturma, Administrator kullanıcısının parola süresini sınırsız yapılması ve dns cachelerinin tetmizlenmesi hata vermeden tamamlanmış olması gerekmektedir.

```text
...

INFO 2020-11-13 06:09:25,458 pid:6414 /opt/samba4/lib/python3.6/site-packages/samba/provision/__init__.py #2032: Setting up sam.ldb rootDSE marking as synchronized
INFO 2020-11-13 06:09:25,478 pid:6414 /opt/samba4/lib/python3.6/site-packages/samba/provision/__init__.py #2037: Fixing provision GUIDs
INFO 2020-11-13 06:09:26,812 pid:6414 /opt/samba4/lib/python3.6/site-packages/samba/provision/__init__.py #2395: A Kerberos configuration suitable for Samba AD has been generated at /opt/samba4/private/krb5.conf
INFO 2020-11-13 06:09:26,812 pid:6414 /opt/samba4/lib/python3.6/site-packages/samba/provision/__init__.py #2396: Merge the contents of this file with your system krb5.conf or replace it with this one. Do not create a symlink!
INFO 2020-11-13 06:09:27,071 pid:6414 /opt/samba4/lib/python3.6/site-packages/samba/provision/__init__.py #2102: Setting up fake yp server settings
INFO 2020-11-13 06:09:27,513 pid:6414 /opt/samba4/lib/python3.6/site-packages/samba/provision/__init__.py #491: Once the above files are installed, your Samba AD server will be ready to use
INFO 2020-11-13 06:09:27,513 pid:6414 /opt/samba4/lib/python3.6/site-packages/samba/provision/__init__.py #495: Server Role:           active directory domain controller
INFO 2020-11-13 06:09:27,513 pid:6414 /opt/samba4/lib/python3.6/site-packages/samba/provision/__init__.py #496: Hostname:              ub18samba
INFO 2020-11-13 06:09:27,513 pid:6414 /opt/samba4/lib/python3.6/site-packages/samba/provision/__init__.py #497: NetBIOS Domain:        ORNEK
INFO 2020-11-13 06:09:27,513 pid:6414 /opt/samba4/lib/python3.6/site-packages/samba/provision/__init__.py #498: DNS Domain:            ornek.lab
INFO 2020-11-13 06:09:27,513 pid:6414 /opt/samba4/lib/python3.6/site-packages/samba/provision/__init__.py #499: DOMAIN SID:            S-1-5-21-2678725650-2705692349-3514259868
Generating RSA private key, 4096 bit long modulus
......................................................................................................................................................................................................................++++
.........................................................................................................................................................................++++
e is 65537 (0x010001)
Generating RSA private key, 2048 bit long modulus
...........................................+++++
.....................................+++++
e is 65537 (0x010001)
Signature ok
subject=CN = ub18samba.ornek.lab
Getting CA Private Key
Expiry for user 'Administrator' disabled.
Created symlink /etc/systemd/system/multi-user.target.wants/samba4.service → /etc/systemd/system/samba4.service.
Rebuilding cache at /opt/samba4/private/dns_update_cache
```



