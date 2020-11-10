## Ders 2 | Bilgi Alma Komutları

# Giriş

Linux sistemler hem arayüz bakımından hem de komut satırı bakımından oldukça gelişmiş sistemlerdir. Hele ki komut satırı. Diğer işletim sistemlerine göre en güçlü terminal yapısına sahip olan işletim sistemi Linux'tur diyebiliriz.  Doğal olarak bu sistemler hakkında terminalden bilgi almaişlemlerini gerçekleştirebiliriz. Bu bilgi alma komutları, sistem hakkında bilgi alma, güncel tarih/saat bilgisi çekme, dağıtım adı, host adı, sistemdeki kullanıcılar ve yetkileri, sisteme bağlı olan çevre birimler hakkında tüm bilgileri komutlar yardımıyla öğrenebiliriz. Şimdi bu komutları inceleyelim.

## lsb_release

Kullandığımız Linux dağıtımının adını öğrenmek için terminalde `lsb_release -a` komutunu çalıştırmamız gerekir. 

![lsb-img1](src)

## uname

Sistemin kullandığı kernel(çekirdek) versiyonunu öğrenmek için `uname -a` komutunu kullanabiliriz. Burada kullandığımız `-a` parametresi `--all` anlamına gelir ve bu parametreyi kullanmak diğer tüm parametreleri birlikte kullanmak için geçerlidir. Bu sayede kernel adı, host adı, çekirdek mimarisi gibi bilgilerin tümünü bir arada görebiliriz. Diğer parametreler ile ayrı ayrı kullanabiliriz.

![uname-img1](src)

## cal

`cal` komutu bir aylık takvimi görüntülemek için kullanabiliriz. Eğer belirli bir a/g/y şeklinde görüntülemek istiyorsak terminale gireceğimiz komut kalıbı; `cal ay yıl` şeklinde olmalıdır. Örneğin, `cal 1 1990` şeklinde komut girdiğimizde 1990 yılının ocak ayını görüntüleyecektir. Eğer belirli bir yıla ait tüm takvimi görüntülemek istiyorsak, `cal 2020` komunutnu kullanabiliriz.

![cal-img1](src)

## date

Sistemin o anki saat ve tarih bilgisini görmek için `date` komutu kullanılır. 

![date-img1](src)

## hostname

Kullandığımız sistemde bilgisayara verdiğimiz adını yani host adını görmek için `hostname` komutunu kullanıyoruz. 

![hostname-img1](src)

## who-whoami

Sistemde kim aktif, kim giriş yapmış, o anki kullanıcı hangi kimlikle çalışıyor gibi çeşitli bilgileri öğrenmek için `w, who, whoami` komutları kullanılabilir.
**w:** Hangi kullanıcının o anda hangi uygulamayı/komutu çalıştırdığı bilgisi,
**who:** Sistemde hangi kimlikle çalıştığı,
**whoami:** Kullanıcının hangi kmlikle çalıştığını gösterir.

![w-img1](src)

## uptime

Sisteminizin ne kadar zamandır açık olduğunu görmek istiyorsanız `uptime` komutunu kullanabilirsiniz.

![uptime-img1](src)

## whereis

Bir dosyayla ilgili çalıştırılabilir dosyanın, kaynak veya yardım dosyasının konumunu almak için `whereis` komutunu kullanabilirsiniz. Kullanım kalıbı `whereis <komut_adı>` şeklindedir. Eğer bu komut parametresiz olarak kullanılırsa direk yanına girdiğiniz komutun dosya yolunu verir. Fakat `-b` parametresi ile kullanıldığında sadece çalıştırılabilir dosyanın yerini, `-m` parametresi ile man sayfasının yerini, `-s` ile de varsa kaynak kodunun yerini gösterir.

![whereis-img1](src)

## which

Parametre olarak verilen bir komutun yol bilgisini yani nerde saklı olduğunu gösterir. Kullanımı, `which <komut_adı>` şeklindedir. Örneğin `which cat` komutunu girdiğimizde çıktı aşağıdaki resimde görüldüğü gibidir. 

![which-img1](src)

## fdisk -l

_fdisk_ komutu aslında diskleri bölümlemek için kullanılan komuttur. Fakat `-l` parametresi ile kullanıldığında sistemin disk bölümleri hakkında detaylı bilgiyi verir. Terminalde, `fdisk -l` komutunu çalıştırdığımızda disk hakkında detaylı bilgiyi görüyoruz.

![fdisk-img1](src)
 
## df

Disk kullanımı ile ilgili ayrıntılı bilgi almak istiyorsak `df` komutunu kullanabiliriz.

![df-img1](src)

## hdparm

`hdparm` komutunu kullandığımızda harddisk hakkında en temel bilgiyi alırız. Net kullanımı, `hdparm /dev/sda` şeklindedir.

![hdparm-img1](src)

## modinfo

Linux'un çekirdek modülleriyle ilgili bilgiye ulaşmak için `modinfo` komutu kullanılır. Örneğin, `modinfo cdrom` komutu çalıştırıldığında cdrom ile ilgili çekirdek modül bilgisine ulaşılır.

![modinfo-img1](src)

## stat

Dosya veya dizin durumu hakkında bilgi almak için `stat` komutu kullanılabilir. 

![stat-img1](src)

## vmstat

Sistemin genel durumunu öğrenmek için kullanılan komut `vmstat` komutudur. 

![vmstat-img1](src)

## Sonuç

Sonuç olarak bu komutlarla sistemimiz hakkında bilgi nasıl alınır onu öğrenmiş olduk. 

[< Önceki Sayfa](https://saricayemre.github.io/linuxkomutsatiridersleri-ders1/) | [Sonraki Sayfa >](https://saricayemre.github.io/linuxkomutsatiridersleri-ders3/)
