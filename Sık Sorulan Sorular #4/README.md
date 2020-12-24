## Sık sorulan sorular - PART 4

**Soru :** OData nedir?  
**Cevap :** Open Data Protocol olarak isimlendirilir. Rest url'ler üzerinden veri kaynaklarını sorgulama protokolüdür.

********************************************************************************

**Soru :** OData dönüş tipi nedir?  
**Cevap :** IQueryable.

********************************************************************************

**Soru :** Caching nedir? Kaç çeşit caching türü vardır?  
**Cevap :** Sık kullanılan ve çok güncellenmeyen verilerin daha hızlı iletilmesi için uygulamanın host edildiği sunucunun belleğinde (In-memory) ya da harici bir sunucuda (Distributed) tutulması tekniğidir. 2 çeşit caching yöntemi mevcuttur. Birisi In-memory diğeri ise Distributed.

********************************************************************************


**Soru :** Cache stratejileri nelerdir?  
**Cevap :** On-demand ve pre-population.


********************************************************************************

**Soru :** Absolute time ve sliding time kavramları nedir? Birlikte kullanılabilir mi?  
**Cevap :** Absolute time verilerin ne kadar süre sonra cache'den silineceğini belirtir. Sliding time ise verilen süre içerisinde veriye erişim gerçekleşmezse cache'ten silinmesini belirtir. İkisi bir arada kullanılabilir. Sliding time değerini 5 dakika olarak belirleyip 5 dakika boyunca veriye erişim olmazsa cache'ten silinmesini istediğimizi belirtebiliriz. Bunun yanında absolute time değerini 30 dakika olarak belirleyip 30 dakika sonrasında ne olursa olsun cache'ten silinmesini istediğimizi belirtebiliriz. Böylece sliding time kullanımından kaynaklanacak eski verileri sürekli gösterme sorununu da çözmüş oluruz.

********************************************************************************


**Soru :** Stack ve Heap kavramları nedir?  
**Cevap :** Yazdığımız kodda tanımladığımız değişkenlerin bellek üzerinde kapladığı alanlardır. Stack kısmında önceden boyutu belli olan değişkenler tutulurken Heap kısmında boyutu değişebilen değişkenler tutulabilir. Stack'te tutulan değerler derleme zamanında oluşturulurken Heap'te tutulan değerler runtime esnasında oluşturulur.

********************************************************************************


**Soru :** JIT (Just In Time) compiler nedir?  
**Cevap :** .Net içerisindeki CLR'ın bir parçasıdır.Microsoft Intermediate language'e derlenen kodları native makine koduna çevirir. Adından yola çıkıp düz mantık ilerleyerek düşünürsek eğer kodumuz tam çalışma anında makine koduna derleniyor (Pre-JIT hariç orda tüm uygulama tek seferde komple derleniyor). Örnek olarak 3 farklı işlem yapan butonların her birine tıklandığında her birisinin kodu tıklanma anında makine koduna çevriliyor.

********************************************************************************


**Soru :** Kaç çeşit JIT mevcut?  
**Cevap :** 3 adet.  
- Pre-JIT Compiler
- Normal JIT Compiler
- Econo JIT Compiler


********************************************************************************

**Soru :** Repository pattern nedir? Ne amaçla kullanılır?  
**Cevap :** Veri yönetiminin tek bir noktaya indirilmesini sağlayan bir tasarım desenidir.


********************************************************************************

**Soru :** IOC Container nedir?  
**Cevap :** IOC yani **I**nversion **O**f **C**ontrol, nesnelerin uygulama süresince yaşam döngüsünden sorumlu olan ve loosely coupled (gevşek bağlı) nesneler oluşturulmasını görev edinen tasarım prensibidir.

********************************************************************************

**Soru :** SOLID nedir?  
**Cevap :** Robert C. Martin tarafından ortaya atılan yazılım prensipleridir. Bu prensiplerin esas amacı uygulamanın daha kolay geliştirilip bakımının sağlanması, yeniden kullanılabilliğin attırılması ve anlaşılabilirliğin yükseltilmesidir. SOLID ultra süper sonik hızlı kodlar yazmanızı sağlamak için oluşturulmuş prensipler değildir. Bu prensiplere harfiyen uyulsa bile inanılmaz yavaş çalışan sistemler geliştirilebilir. Dünyada yapılan her projede kullanılması zorunlu değildir.

- **S** : Single Responsibility
- **O** : Open-Closed Principle
- **L** : Liskov Substitution Principle
- **I** : Interface Segregation Principle
- **D** : Dependency Inversion Principle

********************************************************************************

**Soru :** Single Responsibility nedir?  
**Cevap :** Bir sınıf ya da metodun sadece tek bir görevinin olmasıdır. Bir e-ticaret projesinde Customer sınıfınızda müşterinin adı, soyadı, telefonu vb. şeyler dışında adres bilgisi, önceki siparişleri, kullandığı indirimler, sevkiyat bilgileri gibi bilgilerin tutulmaması bu konuya örnek olarak verilebilir.

********************************************************************************


**Soru :** Open-Closed Principle nedir?  
**Cevap :** Bir sınıfın geliştirmeye açık ancak değiştirilmeye kapalı olması. Şimdi bu cümle okuyunca anlamsız gelebilir o yüzden biraz açıklayalım. Örneğin uygulamanızın loglarını yönettiğiniz bir sınıfınız var diyelim. Siz loglarınızı bir süredir sunucudaki dosyalara yazıyorken sonrasında Elasticsearch gibi bir yapıya yazmak istediniz. Bu durumda gidip loglama yaptığınız sınıfın içeriğini komple Elasticsearch için değiştirirseniz eğer bu kurala uymamış olursunuz. Bunun yerine örneğin ILogger isimli bir interface yaratarak InsertLog() isimli bir metot ekleyerek FileLogger ve ElasticsearchLogger sınıflarında implement edebilirsiniz. Bu sayede sınıflarınızda değişiklik yapmadan farklı çözümler ile loglama yapmaya devam edebilirsiniz.

********************************************************************************


**Soru :** Liskov Substitution Principle nedir?  
**Cevap :**


********************************************************************************

**Soru :** Interface Segregation Principle nedir?  
**Cevap :**

********************************************************************************

**Soru :** Dependency Inversion Principle nedir?  
**Cevap :**

********************************************************************************


**Soru :** Rest Nedir?  
**Cevap :**

********************************************************************************

**Soru :* SqlConnection sınıfı hangi namespace altında yer almaktadır?  
**Cevap :** System.Data.SqlClient

********************************************************************************
