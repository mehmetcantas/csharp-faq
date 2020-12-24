## Sık sorulan sorular - PART 1


**Soru :** C# derlenebilen bir dil midir yoksa yorumlanabilen diller sınıfında mıdır?  

**Cevap :** C# derlenebilen bir dildir.

********************************************************************************

**Soru :** Referans ve değer tipler ne demek? Nasıl çalışır? Her iki tip için de birkaç örnek verebilir misiniz?  

**Cevap :** Değer tipler derlenme anında belleğin Stack bölgesinde oluşturulan tiplerdir. Bu sebeple Garbage Collector tarafından işaretlenemezler işleri bittiğinde yok olurlar. Referans tipler ise belleğin Heap bölgesinde tutulur. Stack bölgesinde ise Heap'teki adresini işaret eden bir pointer oluşturur. Artık kullanılmayan ve boşa düşmüş referans tipler Garbage Collector tarafından temizlenir.  

```
Değer tip örnekleri : int, double, float, Enum
Referans tip örnekleri : Class, Interface, List, String
```

********************************************************************************

**Soru :** Garbage Collector nedir? Kısaca ne iş yapar?  

**Cevap :** Bellekt bir referansı olmayan objeleri temizlemekten sorumlu yapıdır. Garbage Collector çalıştığı esnada çalıştığı Thread dışındaki tüm Threadler durdurulur. 

********************************************************************************


**Soru :** Mutex nedir?  

**Cevap :** Mutual Exclusion kısaltması olarak adlandırılan Mutex'ler uygulamanın dil ve runtime'ı tarafından sağlanan veri yapılarıdır. Ortak paylaşılan bir kaynağa erişimin yönetilmesi görevini üstlenir.

********************************************************************************

**Soru :** Mutex ve Semaphore farklarından birisini söyleyebilir misiniz?  

**Cevap :** Mutex ve Semaphore arasındaki farklardan birisi Mutex'i alan ve bırakan yani release eden Thread aynı olmak zorundadır. Semaphore'da böyle bir gereklilik yoktur.

********************************************************************************

**Soru :** Race condition nedir?  

**Cevap :** Race condition, birden fazla Thread'in aynı anda belleğin aynı kısmına ulaşıp oradaki alanı değiştirmesiyle oluşan durumdur.

********************************************************************************

**Soru :** Bir konsol uygulamasının giriş (entrypoint) metodu hangi metotdur?  

**Cevap :** Main metodu.

********************************************************************************

**Soru :** Main metodunda yer alan string[] args parametresi ne anlama gelir?  

**Cevap :** Komut satırı argümanlarını temsil eder.

********************************************************************************

**Soru :** Managed ve unmanaged code nedir?  

**Cevap :** Managed code doğrudan makine diline derlenmeyen işletim sistemindeki bir servis ya da yorumlayıcı tarafından çalıştırılan kodlardır. Unmanaged code ise doğrudan makine koduna derlenen ve işletim sistemi tarafından çalıştırılan kodlardır. 

********************************************************************************

**Soru :** C# managed olarak mı yoksa unmanaged code olarak mı sınıflandırılır?  

**Cevap :** C# kodları CLR (Common Language Runtime) tarafından MSIL (Microsoft Intermediate Language) olarak derlendiği için managed code olara sınıflandırılır.

********************************************************************************

**Soru :** Statik metotlar override edilebilir mi?  

**Cevap :** Hayır edilemezler.

********************************************************************************

**Soru :** C# içerisinde Namespace kavramı ne anlama gelmektedir?  

**Cevap :** Namespace ilgili sınıflar için bir kapsayıcı görevi üstlenmektedir. Using anahtar kelimesi ile bir Namespace'i başka bir Namespace içerisinde kullanabiliriz.

********************************************************************************

**Soru :** Jagged Arrays nedir?  

**Cevap :** İçerisinde dizi tipinde eleman barındıran dizilerdir. Dizi dizisi (array of arrays) olarak da tanımlanabilir.

********************************************************************************

**Soru :** ++ operatörünün prefix ve postfix olarak kullanımında ne gibi fark vardır?  

**Cevap :** Prefix olarak kullanıldığı durumda önce değeri arttırır ardından fonksiyona gönderir. Postfix olarak kullanıldığında önce değeri fonksiyona gönderir ardından değeri arttırır.

********************************************************************************

**Soru :** == operatörü ile Equals metodu arasındaki fark nedir?  

**Cevap :** == operatörü nesnelerin referanslarını karşılaştırırken Equals metodu nesnelerin içeriğini karşılaştırır.

********************************************************************************

**Soru :** Interface içerisinde statik metot tanımlanır mı?  

**Cevap :** Hayır, tanımlanmaz.

********************************************************************************


**Soru :** Bir class fazla Interface'den miras alabilir mi?  

**Cevap :** Evet alabilir.

********************************************************************************

**Soru :** Statik constructor ne iş yapar?  

**Cevap :** Sınıf örneği alındığı anda statik üyeleri initiliaze etmek için kullanılır.

********************************************************************************

**Soru :** Bir statik metot içerisinde "this" anahtar kelimesi kullanılabilir mi?  

**Cevap :** Hayır, kullanılamaz."this" anahtar sözcüğü bir nesne örneğini işaret eder ancak statik metotlarda bir nesne örneği yoktur.

********************************************************************************


**Soru :** "this" ve "base" anahtar kelimelerinin farkı nedir?  

**Cevap :** "this" içerisinde bulunduğu sınıfı temsil eder. "base" ise parent sınıfı temsil etmektedir.

********************************************************************************

