# Thread_example_Kodluyoruz
**Kodluyoruz Üçüncü-Dördüncü Hafta**

#Dünya Saatleri

Uygulamamızda 5 adet farklı ülkelerin saatlerini göstereceğiz. Şehirler aşağıdaki gibidir.

- Moscow
- Newyork
- London
- Berlin
- New Delhi.

1 - Clock diye bir interfacimiz olacak, bu interfacin showTime() diye bir methodu olacaktır.
2 - City diye ata bir sınıfımız olacak ve her şehir City sınıfından türeyecek. City'nin hem Clock hem de Comparable davranaşı olacaktır. City sınıfına ait özellikler aşağıdaki gibi olacak. City'lerin

- İsmi
- Şehir kodu ( Bu kod dünya üzerinde her şehire ait unique kod olacaktır. https://www.kwe.co.jp/en/useful-contents/code3 bu adresten bulabilirsiniz)
- showTime()
- GMT farkı ( +1, +2, +3)

3- Şehirlerimizi key-value map olarak bir mapte tutacağız. Map'imizin key'i şehir kodlarını tutarken, value kısmı ise Şehirlerimizi tutacaktır.
- Map<String, City>

4- Şehirlerimizi isimlerine göre artan şekilde sıralayabilecek şekilde tasarlayacağız.
5- Uygulama çalıştığında şehirleri isimlerine göre sıralı şekilde kullanıcıya göstererek (Şehir Kodu - Şehir ismi ) kullanıcıdan en az üç en fazla beş olacak  şehir kodu seçmesini isteyeceğiz.
6- Seçilen her şehir için bir Thread açıp, bu threadde sürekli şehirlerin saatlerini anlık olarak göstereceğiz.

NOT: Executor service kullanalım.
NOT2: Runnable interfacini implemente ederek thread yaratalım

EK ÖZELLİK
Kullanıcı dilediğinde tüm programı CTRL+X tuşuna basarak sonlandırabilmeli

