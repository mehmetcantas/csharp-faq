## Sık sorulan sorular - PART 3

**Soru :** Bir değer tipini bir referans tipe dönüştürebilir miyiz? Nasıl?
**Cevap :** Evet dönüştürülebilir. Boxing ve unboxing kullanarak bu işlem gerçekleştirilebilir.


**Soru :** XML case-sensitive midir?
**Cevap :** Evet.

**Soru :** string.Format() içerisinde süslü parantex ({}) nasıl kullanılabilir?
**Cevap :** İki adet süslü parantez daha açıp kapatılarak kullanılabilir.

Örnek : string.Format("FOO BAR BAZ {{{0}}} - {{{1}}},birinciDeger,ikinciDeger);

**Soru :** virtual anahtar kelimesi ne işe yarar?
**Cevap :** Tanımlandığı sınıf haricindeki bir kullanımda bir metodu, property'i ya da event tanımlamasını override edebilmek için kullanılır.


**Soru :** Private virtual metotlar override edilebilir mi?
**Cevap :** Hayır edilemezler. Private metotlar sadece tanımlandığı sınıf içinde erişilebilirler.

**Soru :** Math.Floor() ve Math.Truncate() arasındaki fark nedir?
**Cevap :** Floor() metodu her zaman yukarıya yuvarlar (örneğin 2.5 değerini 3'e) Truncate() metodu ise her zaman sıfıra doğru yuvarlar (örneğin 2.5 değrini 2'ye).


**Soru :** Bir sınıftan miras alınmasını istemiyorsak ne yapmalıyız?
**Cevap :** sealed olarak tanımlanabilir.


**Soru :** Kaç çeşit constructor tipi vardır?
**Cevap :** 5 adet.
- Default
- Parameterized
- Instance
- Static
- Private

**Soru :** Kaç çeşit dizi tipi vardır?
**Cevap :** 3 adet.
- Single dimensional (Tek boyutlu)
- Multi dimensional (Çok boyutlu)
- Jagged (dizi içinde dizi sanki diziception)

**Soru :** try-catch-finally kullanımında hata çıkıp catch bloğu çalışsa bile finally bloğu çalışır mı?
**Cevap :** Evet.

**Soru :** Finally bloğu içerisinde return deyimi kullanılabilir mi?
**Cevap :** Hayır kullanılamaz. Compile hatası verir.


**Soru :** Debug ve Release build'leri arasındaki fark nedir?
**Cevap :** Debug buildleri kodunuzu satır satır debug edebilmeniz için derler. Release buildleri ise uygulamanızın son ve canlıya çıkacak halidir. Release buildlerinde Debug buildlere göre kodunuz daha optimize edilir ve birçok Debug verisi çıkartılır. Bu yüzden Release buildleri Debug buildlere göre daha hızlı çalışır.

**Soru :** .pdb dosyası nedir?
**Cevap :** Açılımı Program Database File olarak geçer. Debug bilgilerini barındırır ve C# ya da VB.NET kodlarınızı Debug modda derlediğinizde oluşur.

**Soru :** Delegate nedir?
**Cevap :** Metod adreslerini saklayan ve parametre olarak metot geçilebilen yapılardır.

Örnek :

```
using System;

namespace test
{
    delegate void calistir();
    class Program
    {
        static void Main(string[] args)
        {
            calistir c = new calistir(EkranaYazdir);
            c += new calistir(OrayaYazdir);
            c += new calistir(BurayaYazdir);
            
            c.Invoke();
        }

        static void EkranaYazdir()
        {
            Console.WriteLine("Ekrana yazdır");
        }


        static void OrayaYazdir()
        {
            Console.WriteLine("Oraya yazdır");
        }

        static void BurayaYazdir()
        {
            Console.WriteLine("Buraya yazdır");
        }
    }
}

```


**Soru :** Abstact sınıflar ile Interface arasındaki farklar nelerdir?
**Cevap :** Kısaca bahsetmek gerekirse;

- Bir sınıf sadece bir abstract sınıfı implement edebilir. Interface'de ise birden fazla Interface implement edilebilir.
- Abstract sınıflar ve sınıflar arasında is-a ilişkisi vardır .Interface ve sınıflar arasında can-do ilişkisi vardır.
- Abstract sınıflar constructor içerebilir, Interface'ler constructor içermezler.
- Interface'ler içi boş metot tanımlamaları barındırabilir bir implementasyon barındıramazlar. Abstract sınıflar her ikisini de barındırabilir.
- Bir sınıf abstract sınıfın belirli bir kısmını implement edebilir ancak Interface'in tamamını implement etmek zorundadır.

**Soru :** .Net içerisinde bir Thread nasıl durdurulabilir?
**Cevap :** İki şekilde. İlki Thread.Interrupt() metodunu kullanarak diğeri ise Thread.Abort() metodunu kullanarak. Buradaki fark Abort kullanımında Thread'in ne yaptığına ya da hangi durumda olduğuna bakmadan durdurması ve bu sebeple istenmeyen sonuçlar oluşturabilmesidir. Interrupt kullanımında ise  ThreadInterruptedException tipinde bir hata fırlatarak Thread'in WaitJoinSleep durumuna geçmesini sağlar.


