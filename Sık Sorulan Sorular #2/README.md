## Sık sorulan sorular - PART 2

**Soru :** Private virtual metotlar override edilebilir mi?  
**Cevap :** Hayır edilemezler çünkü sınıf dışından erişilemezler.

********************************************************************************

**Soru :** Multicast delegate ne iş yapar?  
**Cevap :** Delegate'in bir extension'ı olarak tanımlanabilir. Aynı anda birden fazla metodu işaret etmek için kullanılır.

********************************************************************************

**Soru :** Interface içerisinde private ve protected üyeler tanımlanabilir mi?  
**Cevap :** Tanımlanabilir ancak private üyeler implementasyon esnasında bir anlam ifade etmezler.

********************************************************************************

**Soru :** Bir sınıf birden fazla sınıftan miras alabilir mi?  
**Cevap :** Hayır alamazlar.

********************************************************************************

**Soru :** Bir Array içerisinde birden fazla türde veri saklanabilir mi?  
**Cevap :** Hayır, saklanamaz. Bu tür işlemler için ArrayList ya da object[] kullanılabilir.

********************************************************************************

**Soru :** Bütün Exception sınıflarının base sınıfı hangi sınıftır?  
**Cevap :** System.Exception (LOL)

********************************************************************************

**Soru :** C# içerisinde exception handling nasıl yapılır?  
**Cevap :** try-catch blokları ile.

********************************************************************************

**Soru :** using ifadesi hangi amaçla kullanılır?  
**Cevap :** Using ifadesi dışına çıkıldığı anda objelerin Dispose edilmesi için kullanılır. Bu işlem için ekstra bir kod yazmanıza gerek kalmadan using ifadesi kendi sınırları dışına çıkıldığında Dispose() metodunu çağırır.

********************************************************************************

**Soru :** Catch bloğu kullanılmadan finally kullanılabilir mi?  
**Cevap :** Evet kullanılabilir. Using ifadesi de buna benzer tarzda çalışır.

********************************************************************************

**Soru :** Birden fazla catch bloğu çalışabilir mi?  
**Cevap :** Hayır çalışamaz. Tanımlanabilir ancak oluşan hataya uygun tanımlanmış spesifik bir catch bloğu varsa o çalışır.

********************************************************************************

**Soru :** Immutable nedir?  
**Cevap :** Değiştirilemeyen veri.

********************************************************************************

**Soru :** Reflection nedir?  
**Cevap :** Runtime anında obje ile alakalı metadata bilgilerini almamıza olanak sağlayan yapı.

********************************************************************************

**Soru :** Bir fonksiyondan birden fazla veri döndürülebilir mi?  
**Cevap :** Evet. Bunun için birden fazla yöntem var.

- out parametreleri 
- Class / Struct kullanımı
- Tuple/ Dictionary
- Sıralı bir şekilde dönüş tiplerini belirttiğiniz takdirde aşağıdaki gibi bir kullanım da çalışacaktır.

```
public (int,string,float) TestMethod()
{
    return (1, "test", 1.0f);
}
```
********************************************************************************

**Soru :** ref ve out anahtar kelimelerinin farkı nedir?  
**Cevap :** ref kullanıldığında derleyiciye parametre olarak gönderilen verinin daha önceden bir nesne örneğinin alındığı bilgisi iletilir. out kullanımında ise gönderilen parametrenin iletildiği fonksiyon içinde tanımlanacağı söylenir.

********************************************************************************

**Soru :** System namespace'i hangi dll altındadır?  
**Cevap :** mscorlib.dll

********************************************************************************

**Soru :** Koduma tersine mühendislik (reverse engineering) yapılmasını nasıl önleyebilirim?  
**Cevap :** Kodunuzu obfuscate edebilir yani bir nevi şifreleyebilirsiniz. Dotfuscator isimli araç bu konuda size yardımcı olacaktır.

********************************************************************************

**Soru :** Bir .Net DLL'i içerisinde kaç sınıf barındırılabilir?  
**Cevap :** Sonsuz..

********************************************************************************

**Soru :** int ve System.Int32 arasındaki fark nedir?  
**Cevap :** Fark yok. int System.Int32'nin kısaltılmış bir alias'ıdır.


********************************************************************************
