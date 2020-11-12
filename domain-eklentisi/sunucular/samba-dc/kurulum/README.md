# Kurulum

## Samba Kurulum Yöntemleri

Samba edinmek için 3 adet yöntem bulunmakta. Bunlardan ilki dağıtımların kendi deposundan kurulum yapmak. Bu şekilde kurulduğunda Sambayı ihtiyaca göre elle yapılandırma gerekmektedir. Depolardaki Samba versiyonları dağıtımdan dağıtıma farklılık gösterebilir.

İkinci yöntem Sambayı derleyerek kurmak. Sambanın resmi deposundan kaynak kodları çekilerek derlenebilir. Derlenen Samba, benzer işletim sistemi olmak koşuluyla farklı makinelere de yüklenebilir. Depodan kurulumdaki gibi, ihtiyaca göre yapılandırma gerekmektedir.

Son olarak bizim tarafımızdan derlenen Samba ile, DEB paketini kullanarak rahatlıkla kurulabilir. Derlediğimiz mevcut Samba paketi Debian tabanlı sistemlerde kullanılacak şekilde hazırlanmıştır. Derlediğimiz Samba ile DC yapılandırılması, AD ile migration işlemleri tek komut ile rahatlıkla yapılabilmektedir.

