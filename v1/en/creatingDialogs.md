# Diyalog oluşturmak

Arayüzün sol tarafındaki menüde bulunan `Diyaloglar` sekmesine girin

![leftBar](./src/content6.png)

Sol üst taraftaki `Diyalog Oluştur` butonuna tıklayın

![dialogsPage](./src/content7.png)


## Diyalog İsmi

![createDialogPage](./src/content8.png)

`Diyalog ismi` her bir diyaloğunuza vereceğiniz isimdir. Her diyalog farklı bir isim almalıdır. `Diyalog ismi` sözdizimi boşluk yerine noktalar kullanır ve her noktadan sonra büyük harf ile başlanır. Örn: `test.Dialog1` içinde en az bir nokta kullanan diyaloglar ilk noktadan önce olan kelime ile sınıflandırılır Örneğin eğer `startup.Dialogs1` ve `startup.Dialogs2` olarak iki diyalog kaydederseniz. [Diyaloglar](./dialogs) sayfasında resimdeki gibi görünür.

![leftBar](./src/content11.png)

Fakat eğer ki diyalog isminizi `diyalog1` gibi nokta içermeyen şeklinde oluşturursanız resimdeki gibi görünür

![page](./src/content12.png)

# Diyalogları Bağlama

![connectOtherDialog](./src/content9.png)

Bir sohbette ard arda soracağımız diyalogları birleşitirmek için `Başka diyaloğa bağla` bölümünü kullanırız. Bu kısma ondan sonra devam etmesini istediğimiz [Diyalog ismini](#diyalog-İsmi) gireriz.

> connected.Dialog1 > connected.Dialog2 > connected.Dialog3

gibi. Önemli not: başka diyaloğa bağlı olan diyaloglar algoritma tarafından es geçilirler, sadece bir önceki soru eğer bağlı olan diyaloğun ismine eşitse seçilirler

## Tanımlama Cümleleri

![inputPhrases](./src/content10.png)

Tanımlama cümleleri kullanıcınızın sorusuyla kıyaslanacak cümleler grubudur.

### Örnekler

Tanımlama Cümlesi
> Merhaba ${sys.any}!

Soru
> Merhaba Friday!

Entityler: 

> 'sys.any': 'Friday'

## Entity diyaloglarında yanlışlar

### Yanlış kullanım

 - ${sys.any}${sys.any} nasıldır?
 - İstanbulTürkiye nasıldır?

`sys.any` ard arda kullanılamaz.

### Doğru kullanım

 - ${sys.any}, ${sys.any} nasıldır?
 - İstanbul Türkiye nasıldır?

## Diyalog Yanıtları

![responsegroups](./src/content13.png)

`Diyalog yanıtları` kullanıcı sorusu işlendiğinde tüm yanıtlardan rastgele gelir. Her bir `Diyalog yanıtının` kendi [cevapları](./responses.md) vardır

## Diyalog önizleme

Seçili olan diyalog grubunuzu `Diyalog önzileme` sayesinde sohbette nasıl gözükeceğini görebilirsiniz

![dialogReview](./src/content14.gif)
