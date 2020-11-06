# 2.Hafta Ödev

## Yeni bir Gitthub repository oluştururken, repomuza ekleyebileceğimiz lisanslar nelerdir, bu lisanslar arasındaki farklar nelerdir?

- **MIT**: Projenin ilgili dosyalarının bir kopyasını elde eden herhangi bir kişiye; kullanım, kopyalama, değiştirme ve birleştirme hakları dahil işlem yapma izni vermektedir.
- **Apache**: MIT ile arasında fazla bir fark olmamakla birlikte, projede kullanılan Apache lisanslı ürünlerin lisanslarını da projeyle birlikte dağıtımına eklenmesi gerekmektedir.
- **GNU**: Diğer iki lisansa göre en eski olandır. En önemli farkı GNU  lisansı olan bir ürün ilgili projede kullanıldığında proje dağıtım aşamasına gelirse bu projenin de GNU lisansı olmasını zorunlu kılmasıdır.

## Interface ve Abstract sınıflar arasındaki farklar nelerdir?

- Bir class sadece bir tane abstract class inherit edebilir. Fakat birden çok interface inherit edebilir.
- Bir interface sadece boş gövde barındırır, herhangi bir kod sunamaz.  Abstract classta ise böyle değildir.
- Bir abstract class sub’lar, fonksiyonlar ve property’ler için access modifier’lar içerebilir. İnterface ise içeremez.
- Interface de yeni bir metod yazdığımız zaman bu interfaceden implement ettiğimiz tüm classlarda bu metodun içini tek tek doldurmak gerekiyor ancak abstract classlarda durum farklıdır burada bir metod tanımlayıp içini doldurduğumuzda abstract sınıfımızdan türetilmiş bütün sınıflar bu özelliği kazanmış olur.

## Gang of Four(GOF) araştırınız.

Eric Gamma, Richard Helm, Ralph Johnson ve John Vlissides adında dört yazılımcının;

- İyi bir yazılımı **etkili** bir şekilde nasıl **tasarlayabiliriz** ?
- **Geçmiş** **tecrübelerimizi**, **gelecek** **projelerimize** nasıl aktarabiliriz ?
- Yazılımın tasarımı esnasında, **esneklik** ve **verimlilik** gibi iyi özelliklere nasıl sahip olabiliriz ?

gibi soruları neticesinde 3 kategori ve 23 farklı kalıba dağılmış "Tasarım Kalıp"larıdır. Bu 3 kategori şunlardır;

1- **Creational Patterns**(Kurucu Desenler): Nesnelerin oluşturulması ile ilgili patternlerdir.

2-**Structural Patterns**(Yapısal Desenler): Nesnelerin birbiri ile olan ilişkisini konu alır.

3-**Behavioral Patterns(**Davranışsal Desenler) : Sınıfların bir görevi yerine getirirken nasıl davranacağı ile ilgili desenlerdir.

## Agile-Scrum-Kanban kavramları

- **Agile**, Proje Yönetimi ve Ürün Geliştirme süreçlerini günümüzün çok değişkenli ve dinamik yapısına uyarlayabilmek için geliştirmeci ekiplere sunulmuş prensipler bütünü.
- **Kanban**, esasında olabildiğince işlerimizin görünürlüğüne önem veren, work in progress (WIP) limitini azaltmak ve verimliliği maximize etmek için kullanılan bir framework'tür.
- **Scrum** ekipleri, müşterilere çalışan bir paketi sprint adı verilen belirli aralıklarla göndermeyi taahhüt ederler. Aynı zamanda Agile prensipleri uygulayan diğer framework’ün adıdır.

## Merge - Squash-Rebase arasındaki farklar nelerdir?

**Rebase**: Master a bir branch i rebase ettiğinizde , branch deki commitlerinizi tek tek alıp master ın sonuna ekler.Rebase sonucunda tek bir history oluşturur çünkü tamamlanan işi bir branch ten diğerine aktarır. Bu süreçte istenmeyen history ortadan kalkar.

**Merge**:Merge yaptığmızda is yeni bir “ Merge commit” yaratıp iki branchinde tüm history sini içerecektir. Master , branch te yapılan tüm değişiklikleri alacak ve entegre edecektir ancak branch in history sinde hiçbir değişiklik olmayacaktır.

**Squash**: Bir birleştirme talebini kabul ederken  branch' ın commit history sini düzenlemenizi sağlar. Birleştirme isteğindeki tüm değişiklikleri tek bir commit olarak uygular.

