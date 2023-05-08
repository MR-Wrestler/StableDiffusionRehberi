2i# txt2image (md)

![text2image](https://i.imgur.com/8D5GGIO.png)

## Prompt:

- Prompt bölümü Stable Diffusion da oluşturmak istediğiniz resimde olmasını istedğiniz özellikleri girdiğiniz bölümdür. 
Kullanılan promplar ve çıktılarının yayınlandığı birçok site mevcuttur. Bazıları:
    
    [Prompthero](https://prompthero.com/stable-diffusion-prompts)
    [Lexica](https://lexica.art/)
    [Openart](https://openart.ai/discovery)
    [CivitAI](https://civitai.com/)
    [Stable Diffusion Art](https://stable-diffusion-art.com/prompts/) 
    !!DİKKAT!!
    Bu sitelerdeki bazı resimler +18 içerikte olabilir.
    
- Stable Diffusion v2 ve daha üst versiyonlar telif hakları nedeniyle sanatçıların görsel modelleriyle beslenmeye kapatılmıştır. Yani “Greg Rutkowski tarzı çizim yap” şeklinde bir propmt girildiğinde devreye alınmkayacaktır. Ama daha alt versiyonlarda böyle bir sıkıntı yoktur.

Prompt kısmına ayrı bir rehber hazırlamayı düşünüyorum o yüzden şimdi çok detaylı olarak değinmeyeceğim. Rehberi hazırladığımda linkini burada da paylaşırım.

## Negative Prompt:

- Stable Difusion da oluşturmak istediğiniz resimde olmamasını istedğiniz özellikleri girdiğiniz bölümdür.

## Sampling Method

- Görüntünün oluşumunda rol alan metodu belirtir. Her Sampling Method’un farklı özellikleri vardır.

## Sampling Steps

- Oluşturlacak olan resimdeki detay seviyesi olarak düşünülebilir. Sampling Steps ne kadar yüksek olursa resim o kadar detaylı olur. Bununla birlikte resmi oluştırmak için gereken süre de artar.

## Restore Faces

- Yüzlerdeki kusurları onarmak için bu özelliği açabilirsiniz. (Çoğu modelde modelin yüz yaratma kodlarıyla çakışıp sıkıntı çıkarabiliyor. O yüzden kullanılması çok tavsiye edilmiyor.)

## Tiling

- Girdiğiniz prompttan bir desen oluşmasını istiyorsanız bu özelliği açabilirsiniz.

## Hires Fix

- Yüksek parametreli görseller yaparken oluşabilecek hataları düzeltmeye yarar.
- Çalışmasındaki temel prensip:
    
    Ayarladığımız Sampling Steps değerinin yarısına gelindiğinde Hires Fix seçeneği açık ise görsel oluşturma süreci yeniden başlar. Böylece oluşan nihai resim 2 kere kontrol edilmiş olur. Bu sayede hataların önüne geçilmeye çalışılır.
    
- Düşük çözünürlükte Hires Fix seçeneği seçildiği zaman bozuk görseller alabilirsiniz.

## Width and Height

- Oluşturulacka olan görselin boyutlarının ayarıdır.
- Stable Diffusion v1.5 ve v1.4 modellerinin oluşturulmasında kullanılan referans görselleri 512x512 boyutlarındadır.
- Stable Diffusion v2.0 ve v2.1 modellerinin oluşturulmasında kullanılan referans görselleri 768x768 boyutlarındadır.
- Bu modellere referans çözünürlüklerinden daha yüksek çözünürlükte görsel oluşturmak isterseniz hatalar (piksel kaymaları, 2 3 tane kafa oluşması vb) ile karşılaşabilirsiniz.)
- Aşağıdaki Tabloda Sosyal medya platformlarında kullanılan görsel boyutlarının tablosu verilmiştir:
    
    
    | Platform | Özellik | Boyut |
    | --- | --- | --- |
    | Instagram | Profil Fotoğrafı | 110 x 110 px |
    | Spotify | Profil Fotoğrafı | 750 x 750 px |
    | Instagram | Gönderi (kare) | 1080 x 1080 px |
    | Instagram | Gönderi (yatay) | 1080 x 650 px |
    | Instagram | Gönderi (dikey) | 1080 x 1250 px |
    | Instagram | Hikaye (9:16) | 1080 x 1920 px |
    | Instagram | Reels ve Video (9:16) | 1080 x 1920 px |
    | Spotify | Çalma Listesi Kapağı | 640 x 640 px |
    | Facebook | Profil Fotoğrafı | 180 x 180 px |
    | Facebook | Kapak Fotoğrafı | 820 x 312 px |
    | Facebook | Gönderi (dikdörtgen) | 1200 x 630 px |
    | Facebook | Gönderi (kare) | 1200 x 1200 px |
    | Facebook | Hikaye | 1080 x 1920 px |
    | Twitter | Kapak Fotoğrafı | 1500 x 500 px |
    | Twitter | Profil Fotoğrafı | 400 x 400 px |
    | Twitter | Paylaşım Görseli | 1024 x 512 px |
    | Pinterest | Profil Fotoğrafı | 165 x 165 px |
    | Pinterest | Standart Pin | 600 x 900 px |
    | Pinterest | Uzun Pin | 600 x 1260 px |
    | Pinterest | Kare Pin | 600 x 600 px |
    | LinkedIn | Profil Fotoğrafı (kişisel hesaplar) | 400 x 400 px |
    | LinkedIn | Profil Fotoğrafı (şirket hesapları) | 300 x 300 px |
    | LinkedIn | Kapak Fotoğrafı (şahıs) | 1584 x 396 px |
    | LinkedIn | Kapak Fotoğrafı (şirket) | 1536 x 768 px |
    | LinkedIn | Paylaşım Görseli | 1104 x 736 px |
    | Youtube | Kanal Profil Fotoğrafı | 800 x 800 px |
    | Youtube | Kapak Fotoğrafı | 2560 x 1440 px |
    | Youtube | Video Thumbnails | 1280 x 720 px |

## Batch Count

## Batch Size

- Yapay zeka’nın bir seferde oluşturacağı görsel sayısını gösterir.

## CFG Scale

- Girilen propmtun oluşturulacak olan görsele ne kadar etki edeceğinin ayarıdır.
- CGF Scale yüksek değerde seçilirse daha kontrastlı renkler kullanılacaktır.

## Seed

- Seed dediğimiz değer, rastgelelik değeri gibi düşünülebilir. (Minecraftdaki random oluşturulan her dünya birbirinden farklıydı ve eğer birisi sizin oluşturduğunuz dünyanın aynısını oluşturnak isterse sizin dünyanızın seed ini girmesi gerekir. Stable Diffusionda da benzer bir mantk kullanılmaktadır.)
- Eğer seed parametresi -1 olduğunda propt ve diğer değerler aynı kalsa bile farklı görseller oluşturulmaktadır.
- Eğer oluşturduğunuz görselin seed ini seed kısmına yazmak istiyorsanız :recycle: emojisine tıklayabilirsiniz.

## Script

Automatic 1111 Web arayüzünü kullanarak stable diffusion üzerinde ekstra kodlar çalıştırabilmenizi sağlar. 

Scripler için de ayrı bir rehber hazırlamayı düşünüyorum linkini buraya ekleyeceğim.
