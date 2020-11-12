# Proxmox üzerinde USB başlatma

1. Kurulu bir Proxmox ortamınız bulunmakta ise Depolama birimine ISO'yu yüklediyseniz, Proxmox arayüzünden "Create VM" butonuna tıklayarak yeni bir sanal makine oluşturmaya başlabilirsiniz. Anlaşılır bir isim vererek bir sonraki adıma geçebilirsiniz.

![](../../../.gitbook/assets/screenshot-from-2020-06-14-20-43-42.png)

1. OS \(İşletim Sistemi\) sekmesinde CD aygıtı olarak depolama alanına yüklediğiniz ISO'yu seçmeniz gerekmektedir.

![](../../../.gitbook/assets/screenshot-from-2020-06-14-20-44-31.png)

1. Sistem sekmesinde herhangi bir değişiklik yapmadan ilerleyebilirsiniz.
2. Hard Disk sekmesinde ise hangi depolama alanına kurulum yapacaksanız o kısmı seçmeniz gerekmekte ve yaklaşık 50 GB'lık bir disk boyutu seçebilirsiniz.

![](../../../.gitbook/assets/screenshot-from-2020-06-14-20-46-20.png)

1. CPU sekmesinde 1 soket, 2 core seçerek ilerleyebilirsiniz.

![](../../../.gitbook/assets/screenshot-from-2020-06-14-20-47-24%20%281%29.png)

1. Hafıza sekmesinde 2048 MiB değeri seçip ilerleyebilirsiniz.

![](../../../.gitbook/assets/screenshot-from-2020-06-14-20-48-16.png)

1. Ağ sekmesinde de mevcut durumdaki ile aynı şekilde ilerleyebilirsiniz.

![](../../../.gitbook/assets/screenshot-from-2020-06-14-20-48-43.png)

1. Son olarak onaylama sekmesinde özet bilgileri inceleyerek alttaki "Start after created"'i işaretleyerek oluşumdan sonra açılmasını sağlayabilirsiniz.

![](../../../.gitbook/assets/screenshot-from-2020-06-14-20-49-19.png)

1. Bu adımdan sonra Proxmox üzerinde VM listesinde Sanal Makina'nızın ayağa kalktığını görebilirsiniz.

