# Depo üzerinden kurulum

Liman'ı en verimli şekilde kurmanın yöntemi depo üzerinden kurulumdur. Bunun için aşağıdaki adımları uygulamak gerekmektedir.

## 1. Aciklab deposunu eklemek

Depo üzerinden Liman MYS kurmak için öncelikle Liman'ın bulunduğu AcikLab deposunu sisteminize eklemeniz gerekmektedir. Öncelikle aşağıdaki komut ile depo adresini paket kaynak listenize eklemelisiniz:

```text
echo "deb [arch=amd64] http://depo.aciklab.org/ onyedi main" | sudo tee /etc/apt/sources.list.d/acikdepo.list
```

Depoyu ekledikten sonra kullanabilmek için AcikLab deposu için public.key'i sisteminize güvenilir şekilde eklemeniz gerekmektedir. Aşağıdaki komut ile açık anahtarı sisteminize ekleyebilirsiniz:

```text
sudo wget -qO - http://depo.aciklab.org/public.key | sudo apt-key add -
```

## 2. Güncel Liman'ı depo üzerinden yüklemek

Bu adımdan sonra sisteminizi güncelledikten sonra liman MYS'yi yükleyebilirsiniz:

```text
sudo apt update
sudo apt install liman
```

## 3. Yönetici kullanıcısı oluşturmak

Kurulum sonrasında ilk yapılması gereken Yönetici parolası oluşturmak. Bunun için aşağıdaki komutlar ile sudo yetkili kullanıcıda iken liman kullanıcısına giriş yapılır ve yönetici hesabı oluşturulur:

```text
sudo su liman
sudo php /liman/server/artisan administrator
```

Bu adım sonunda karşınıza liman web arayüzünden giriş yapacağınız kullanıcı adı ve parolanız çıkacaktır. Liman'ı kurduğunuz sunucunun ip adresini web tarayıcınız üzerine yazıp bu bilgiler ile giriş yaparsanız Liman'ın Web arayüzüne giriş yapmış olacaksınız.

![](../../.gitbook/assets/screenshot-from-2020-06-14-18-58-36%20%281%29.png)

