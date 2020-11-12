# VirtualBox üzerinde USB başlatma

Herhangi bir işletim sisteminde VirtualBox uygulamasını açmanız ve uygulama açıldıktan sonra aşağıdaki gibi yeni bir Sanal Makine oluşturma ikonuna tıklamanız gerekmektedir. Aynı işlemi menübar'da Makine&gt;Yeni menüsüne basarak da oluşturabilirsiniz.

![VirtualBox 6.0 aray&#xFC;z&#xFC;](../../../.gitbook/assets/ekran-goeruentuesue_2020-03-07_23-02-15.png)

Yeni butonuna basıldıktan sonra sizden kendi tanımanız için gerekli bir isim, sanal makineyi hangi dizine kuracağınız bilgisi ve daha sonra "misafir eklentileri" denilen VirtualBox üzerinde ek ayarlar yapmanıza izin veren yapıyı kullanmak için işletim sistemi seçmenizi isteyecektir. Herhangi bir isim girip diğer ayarları aynı tutmanızda herhangi bir problem olmayacaktır. Fakat yazdığınız isme göre işletim sistemi otomatik tanımaya çalışacağı için "Linux&gt;Other Linux" seçmeniz uygun olacaktır.

![Sanal Makine Olu&#x15F;turma ana ekran](../../../.gitbook/assets/ekran-goeruentuesue_2020-03-07_22-54-00.png)

İleri dedikten sonra sizden sanal makineniz için RAM ayırmanızı isteyecektir. Bu sistem gerçek bir ortam olmayacağı için tahminen en düşük 1300 MB olacak şekilde 2048 MB veya 4096 MB gibi değerler verebilirsiniz. Tabi ki tüm bu değerler VirtualBox'u kurduğunuz makinedeki RAM'den kullanacağı için kendi kullandığınız RAM değerine göre bir oran vermeniz gerekmektedir. Ayrıca bu ayarı sanal makine kapalı olduğu herhangi bir an ileride değiştirebilirsiniz. Makine açık ise kapattıktan sonra değiştirebileceğinizi unutmayın.

![Sanal Makine Bellek Boyutu](../../../.gitbook/assets/ekran-goeruentuesue_2020-03-07_22-54-16.png)

Oluşturacağınız sanal makineye bir de sanal disk eklemeniz gerekmektedir. Bunun için daha önce bir disk oluşturmadığınızı düşünerek "Şimdi sanal bir disk oluştur" seçeneğini seçmenizin uygun olacağını belirtirim. Boyutunu ise ileriki kısımlarda düzenleyebileceksiniz. Ayrıca sanal makinenize ek diskler eklemek için ileride sanal makine kapalı iken istediğiniz sayıda disk ekleyebilirsiniz.

![Sanal Makine Sabit Disk](../../../.gitbook/assets/ekran-goeruentuesue_2020-03-07_22-54-26.png)

Yeni bir sabit disk oluşturduğunuz için sanal disk türü belirlemeniz gerekmektedir. Varsayılan olarak seçili gelen VDI \(Virtualbox Disk Kalıbı\) seçebildiğiniz gibi, VHD ve VMDK gibi sanal disk türlerini seçebilirsiniz. Bu formatlar Microsoft ve VMware'in sanallaştırmada kullandığı disk imajları olarak düşünebilirsiniz. İleride risk oluştursa da vdi'dan vmdk ve vhd'ye geçiş yapabilirsiniz.

![Sanal Sabit Disk T&#xFC;rleri](../../../.gitbook/assets/ekran-goeruentuesue_2020-03-07_22-54-35.png)

Sanal diskinizin gerçek disk üzerinde tümünün ayrılmış olarak mı yoksa arttıkça mı yer kaplayacağını seçmeniz gerekmektedir. Buradaki tercih en çok kısıtlı disk alanlarında kullanıma göre değişmektedir. Çok önemli bir sunucu ise sabitlenmiş boyut seçerek bir sonraki pencerede seçeceğiniz boyutta sanal disk alanını gerçek disk üzerinde de ayırır. Böylelikle ileride disk dolması durumunda sanal makinede problem olmasını engelleyecektir.

![Fiziksel diskte depolama se&#xE7;enekleri](../../../.gitbook/assets/ekran-goeruentuesue_2020-03-07_22-54-43.png)

Sanal diskin fiziksel disk üzerinde hangi dizinde tutulacağı ve boyutunun ne kadar olacağını seçeceksiniz. Hızlı bir uygulama istiyorsanız ve fiziksel işletim sisteminizde SSD bulunuyor ise bu alanı seçmeniz daha uygun olacaktır. İşletim sistemi için minimum olarak 8 GB yer ayırmanız uygun olacaktır. Örnekte 88 GB seçilmiştir.

![Sanal diskin yeri ve boyutu](../../../.gitbook/assets/ekran-goeruentuesue_2020-03-07_22-55-29.png)

Bu adımdan sonra sanal makineniz temel seviyede oluşturulmuş olacaktır ve tekrar VirtualBox ana ekranına düşeceksiniz. Bu ekranda sol tarafta kendi verdiğiniz isimdeki sunucuya bastıktan sonra sağ kısımda ayarlara basabilirsiniz. Veya menübarda Makine&gt;Ayarlar kısmına basmanız gerekmektedir.

![VirtualBox ana ekran&#x131;](../../../.gitbook/assets/ekran-goeruentuesue_2020-03-07_22-57-12.png)

Açılan pencerede solda "Depolama" tabına giriş yaptıktan sonra CDROM işareti olan ve Boş gözüken kısma tıklayıp, sağ kısımda yine CDROM ikonuna tıklayarak sanal makinenize daha önce [Kuruluma Giriş](../../kurulum-giris.md) bölümünde anlatılan Pardus Sunucu USB kalıbını \(.ISO formatındaki\) seçmeniz gerekmektedir.

![CDROM Kal&#x131;b&#x131;n&#x131;n sanal makineye eklenmesi](../../../.gitbook/assets/ekran-goeruentuesue_2020-03-07_22-57-31.png)

![Pardus Sunucu imaj&#x131;n&#x131;n se&#xE7;ilmesi](../../../.gitbook/assets/ekran-goeruentuesue_2020-03-07_22-57-49.png)

Ve sonunda aşağıdaki gibi pencerede CDROM olarak Pardus Sunucu imajının seçili olması gerekmektedir. İlgili ekranda **Tamam**'a tıklayarak sanal makine CDROM'dan başlayacak hale getirilmiştir.

![](../../../.gitbook/assets/ekran-goeruentuesue_2020-03-07_22-58-15.png)

Bir sonraki adımda aşağıdaki gibi pencere üzerinde solda kurduğunuz sanal makine adına tıkladıktan sonra üstte Başlat'a veya menübar üzerinden Makine&gt;Başlat'a tıklayarak [Kurulum Süreçleri](../../kurulum-surecleri/)'nde bahsedilen süreçler için sanal makinenizde kuruluma geçebilirsiniz.

