# Java Veri Tipleri

Değişkenler, verileri hafızada belli bir alan içinde tutmaya, saklamaya yararlar. Her değişken tanımı yapılırken bir veri tipi belirtilir. Veri tipine göre de değişken tanımlandığı esnada hafızada ne kadar yer kaplayacağı belli olur.

Java&#39;da iki tip değişken grubu vardır:

- İlkel Veri Tipleri (Primitive Data Types)
- Nesne Veri Tipi (Object Data Types)

![](figures/veri-tipleri-1.png)

## İlkel Veri Tipleri

Java&#39;da dille birlikte tanımlı olarak gelen 8 adet ilkel veri tipi vardır.

- boolean
- int
- char
- byte
- short
- long
- float
- double

| **Veri Tipi** | **Varsayılan Değeri** | **Veri Boyutu** |
| ------------- | --------------------- | --------------- |
| boolean       | false                 | 1 bit           |
| char          | &#39;\u0000&#39;      | 2 byte          |
| byte          | 0                     | 1 byte          |
| short         | 0                     | 2 byte          |
| int           | 0                     | 4 byte          |
| long          | 0L                    | 8 byte          |
| float         | 0.0f                  | 4 byte          |
| double        | 0.0d                  | 8 byte          |

### &quot; **boolean&quot; Veri Tipi**

Bu veri tipinde sadece iki değer tutabiliriz. &quot;true&quot; veya &quot;false&quot; şeklinde iki değere sahiptir. Hafızada 1 Bit büyüklüğünde yer kaplar.

Örnek Tanımlama:

````java
boolean printerEnabled = false ;
````



### &quot; **byte&quot; Veri Tipi**

-128 ile 127 arasında değer alabilen sayısal bir tam sayı tipidir. Varsayılan değeri sıfırdır. Özellikle, hafızada az yer kaplaması nedeniyle kullanılabilir. Eğer, &quot;int&quot; tipine gerek duymuyorsanız, &quot;byte&quot; kullanmak faydalı olacaktır.

Örnek Tanımlama:

````java
byte humanAge =32;
````



### &quot; **short&quot; Veri Tipi**

16 Bit&#39;lik (yani 2 Byte) veri büyüklüğüne sahip tam sayı veri tipidir. -32,768 ile 32,767 arasında değer alabilir. Varsayılan değeri sıfırdır. Yine &quot;int&quot; veri tipine ihtiyaç duymadığınız zaman &quot;short&quot; tipte değişkenler oluşturarak hafızadan kazanç sağlayabilirsiniz.

Örnek Tanımlama: 

````java
short m2OfRegion =11991;
````



### &quot; **int&quot; Veri Tipi**

32 Bit&#39;lik (yani 4 Byte) veri büyüklüğüne sahip tam sayı veri tipidir. - 2,147,483,648 ile 2,147,483,647 arasında değer alabilir. Varsayılan değeri sıfırdır. &quot;int&quot; tipinde değişken tanımlarken gerçekten o kadar büyüklüğe sahip bir veri tutacak mıyız, iyi kontrol etmek gerekir. Örneğin: insan yaşı bilgisini &quot;int&quot; veri tipinde tutmak hafızada fazladan alan kaplamak demek olacaktır. Zaten insan yaşı &quot;int&quot; değerinden çok küçüktür. Bunun için &quot;byte&quot; tipinde bir değişken tanımlamak hafızayı etkin kullanmayı sağlayacaktır.

Örnek Tanımlama:

````java
int bookCountInWorld =1199221;
````



### &quot; **long&quot; Veri Tipi**

64 Bit&#39;lik (yani 8 Byte) veri büyüklüğüne sahip tam sayı değeridir. Tam sayı veri tipleri içinde en büyük değer aralığına sahip veri tipidir. Çok büyük basamaklı sayıları tutabilmek için idealdir. Hafızada önemli bir yer kaplar. Kullanırken dikkatli olmak gerekir.

-9,223,372,036,854,775,808 ile 9,223,372,036,854,775,807 arasında değer alabilir.

Örnek Tanımlama:

````java
long galaxyCountInSpace =51992212222;
````



### &quot; **float&quot; Veri Tipi**

32 Bit&#39;lik (yani 4 Byte) veri büyüklüğüne sahip ondalıklı sayı değeridir. Sayı aralığına bir limit getirilmemiştir. Hafızayı etkin kullanmak adına &quot;double&quot; veri tipi yerine tercih edilebilir. Çünkü, &quot;double&quot; veri tipi &quot;float&quot; &#39;dan daha büyük bir yer kaplamaktadır. Varsayılan değeri 0.0F şeklindedir. Float tipindeki değişkenlere atanan verilerin sonunda &quot;f&quot; son eki vardır. Değişkene atanan değerin &quot;float&quot; tipinde olduğunu belirtir.

Örnek Tanımlama:

  ````java
float freezeRatio =3.23f;
  ````



### &quot; **double&quot; Veri Tipi**

64 Bit&#39;lik (yani 8 Byte) veri büyüklüğüne sahip ondalıklı sayı değeridir. Sayı aralığına bir limit getirilmemiştir. Boyutu büyük olduğu için tanımlama yapılırken gerçekten &quot;float&quot; veri tipinin yetersiz olduğu durumlarda kullanılmalıdır. Varsayılan değeri 0.0d şeklindedir. Atanan verinin sonuna &quot;d&quot; son eki koyularak &quot;double&quot; tipte bir veri olduğu belirtilebilir. Fakat, &quot;d&quot; son ekinin koyulmadığı durumlarda ondalıklı sayı verisi varsayılan olarak &quot;double&quot; olarak kabul edilir. Konulması zorunlu değildir.

Örnek Tanımlama: 

````java
double freezeRatio =3.2322;
````



### &quot; **char&quot; Veri Tipi**

16 Bit&#39;lik (yani 2 Byte) büyüklüğüne sahip karakter verilerini tutar. Unicode tipinde karakter verilerini saklar. &#39;\u0000&#39; (0) ile &#39;\uffff&#39; (65535) aralığında değer alır.

Örnek Tanımlama:

``````java
char letter = 'A';

char letter = 'B';

char letter = 'C';
``````



## Unicode Karakter Sistemi

Bilgisayar dünyasında karakterler sayısal ifadeler ile temsil edilir. Aslında, her harfin veya sembolün bir sayısal karşılığı vardır. Dünyadaki çoğu dile ait karakterleri tanımlayan sisteme Unicode Karakter Sistemi denir.

Unicode sistemi dışında kullanılan diğer karakter sistemleri:

- **ASCII** (American Standard Code for Information Interchange)
- **ISO 8859-1** (Batı Dilleri için)
- **KOI-8** (Rusça için)
- **GB18030** ve **BIG-5** (Çince ve diğer diller için)

Unicode sistemi ile tüm dillere ait karakterler 2 Byte şeklinde tanımlandığı için uluslararası bir standarda sahiptir. Bu nedenle Java tarafından tercih edilmiştir. Diğer karakter sistemlerinden birbirine dönüşüm yapmak sorunlu ve maliyetli bir iştir.

| **Notasyon** | **Temsil Eden Karakter**             |
| ------------ | ------------------------------------ |
| \n           | Yeni satır (0x0a)                    |
| \r           | Satırbaşı (0x0d)                     |
| \b           | Geri tuşu (0x08)                     |
| \s           | Boşluk (0x20)                        |
| \t           | Bir tab Boşluk                       |
| \ "         | Çift Tırnak Kaçış Karakteri          |
| \ '        | Tek Tırnak KaçışKarakteri            |
| \ \        | Ters slash karakteri                 |
| \uxxxx       | Hexadecimal UNICODE Karakteri (xxxx) |