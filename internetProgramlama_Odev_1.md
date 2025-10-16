
## 1\. İnternetin temel çalışma prensibini kısaca açıklayınız.

Cevap: Bilgisayarlar ag uzerinden konusur. Paketler gonderir alir. TCP/IP protokolleri kullanir. Routerlar yonlendirir. Veri parcalara bolunur, karsida birlestirilir.

## 2\. IP adresi ve DNS arasındaki farkı açıklayınız.

Cevap: IP adres, bilgisayarin agdaki numarasi. 192.168.1.1 gibi. DNS ise https://www.google.com/search?q=google.com gibi isimleri bu numaralara cevirir. Insanlar isim hatirlar, makinalar numara kullanir.

## 3\. TCP ve UDP arasındaki farkları belirtiniz.

Cevap: TCP guvenli baglanti. Veri sirali gider, kayip olursa tekrar gonderir. Yavas. UDP hizli. Veri gonderir, ulasip ulasmadigi onemli degil. Kayip olur. Oyun, video gibi.

## 4\. HTTP protokolü hangi katmanda çalışır ve temel özellikleri nelerdir?

Cevap: HTTP, Uygulama katmaninda calisir (OSI 7. katman). Temel ozelligi web sayfalari getirmek. Istek (request) ve cevap (response) mantigi var. Durumsuz (stateless) protokoldur, eski istekleri hatirlamaz.

## 5\. Web tarayıcıları nasıl çalışır? Bir web sayfasını yükleme sürecini adım adım açıklayınız.

Cevap: Adresi yazarsin (https://www.google.com/search?q=google.com). Tarayici DNS’e sorar, IP alir. O IP’ye HTTP istegi gonderir. Sunucu HTML, CSS, JS dosyalari gonderir. Tarayici bu dosyalari okur, isler ve ekrana cizer (render). Sayfa gorunur.

## 6\. Frontend ve Backend arasındaki fark nedir? Örneklerle açıklayınız.

Cevap: Frontend kullanicinin gordugu kisim. Butonlar, yazilar. HTML, CSS, Javascript. Backend arka plan. Veritabani, sunucu mantigi. Kullanici gormez. Python, Go, Java. Ornek: Facebook’ta gordugun begen butonu frontend, begeninin kaydedilmesi backend.

## 7\. JSON ve XML arasındaki farkları açıklayınız.

Cevap: Ikisi de veri tasir. JSON daha basit, kisa. { "ad": "Kaan" } gibi. Javascript’e yakin. XML daha cok etiket kullanir. \<ad\>Kaan\</ad\> gibi. XML daha karmasik ama kuralli. JSON daha hizli.

## 8\. Restful API nedir? Ne amaçla kullanılır?

Cevap: RESTful API, sunucuyla konusmak icin bir yontem. Kurallar butunu. HTTP metodlari kullanir (GET, POST, PUT, DELETE). Veri almak, eklemek, silmek icin. Genelde JSON formatinda veri doner. Servislerin birbiriyle konusmasini saglar.

## 9\. Güvenli internet iletişimi için kullanılan HTTPS protokolünün avantajlarını açıklayınız.

Cevap: HTTPS guvenlidir. HTTP’nin S’li hali. Veriyi sifreler. Araya girenler veriyi okuyamaz. Banka siteleri, e-ticaret hep bunu kullanir. Yesil kilit gorursun tarayicida. SSL/TLS sertifikasi kullanir.

## 10\. Çerezler (Cookies) nedir? Web sitelerinde nasıl kullanılır?

Cevap: Cerezler kucuk bilgiler. Tarayicida saklanir. Site seni hatirlar. Oturum acik kalir, sepete eklediklerin unutulmaz. Sunucu cerezi gonderir, tarayici saklar. Sonra her istekte geri gonderir.

# Bölüm 2: HTML ve CSS Örnek Soruları

## 1\. Aşağıdaki HTML kodunun çıktısını tahmin ediniz:

```html
<!DOCTYPE html>
<html>
<head>
<title>Örnek Sayfa</title>
</head>
<body>
<h1>Merhaba Dünya!</h1>
<p>Bu bir paragraf.</p>
<a href="https://www.google.com">Google'a git</a>
</body>
</html>
```

Cevap: Ekranda buyuk bir baslik "Merhaba Dunya\!" yazar. Altinda "Bu bir paragraf." yazar. En altta "Google'a git" yazan bir link olur, tiklayinca [https://www.google.com](https://www.google.com)’a gider.

## 2\. \<div\> ve \<span\> etiketleri arasındaki farkı açıklayınız.

Cevap: \<div\> blok etikettir. Tum satiri kaplar. Ogeleri gruplamak icin kullanilir. \<span\> satir ici (inline) etikettir. Sadece icindeki yazi kadar yer kaplar. Bir kelimeyi falan ayirmak icin.

## 3\. HTML’de form elemanlarından en az 5 tanesini açıklayınız.

Cevap: `<input type="text">`: Kucuk yazi kutusu. `<input type="password">`: Sifre kutusu, yazilar nokta gorunur. `<input type="submit">`: Formu gonderme butonu. `<textarea>`: Buyuk yazi alani. Adres falan. `<select>`: Acilir liste. Icinde `<option>` olur.

## 4\. CSS’te ID ve Class seçicilerinin farkı nedir? Örnek kod vererek açıklayınız. Aşağıdaki CSS kodu hangi elementlere uygulanır?

```css
p {
color: red;
font-size: 16px;
}
```

Cevap: ID bir sayfada tek olmali. Benzersiz. CSS’te \# ile secilir (\#baslik). Class cok olabilir. Ayni stili bircok ogene verir. CSS’te . ile secilir (.paragraf). Ornek:
HTML: `<p id="ana" class="kutu">Yazi</p> <p class="kutu">Yazi 2</p>`
CSS: `#ana { color: blue; } .kutu { border: 1px solid black; }`

Verilen CSS kodu `p { ... }` sayfadaki tum `<p>` (paragraf) etiketlerine uygulanir. Onlari kirmizi ve 16 piksel yapar.

## 5\. HTML5’te yeni gelen en az 3 etiketi açıklayınız.

Cevap: `<header>`: Sayfanin ust kismi, baslik, logo falan. `<footer>`: Sayfanin alt kismi. Iletisim, linkler. `<nav>`: Navigasyon, menu linkleri icin.

## 6\. CSS Flexbox ile bir div öğesini yatay ve dikey olarak nasıl ortalarsınız?

Cevap: Ortalanacak div’in ana (parent) div’ine su kodlar yazilir:

```css
.ana-div {
  display: flex;
  justify-content: center; /* Yatay ortalama */
  align-items: center;    /* Dikey ortalama */
}
```

## 7\. Responsive web tasarım nedir? Örnek bir CSS media query yazınız.

Cevap: Responsive tasarim, sitenin her ekranda (telefon, tablet, pc) duzgun gorunmesi. Ekran boyutuna gore tasarim degisir. Media query ile yapilir. Ornek:

```css
@media (max-width: 600px) {
  .menu {
    display: none; /* Ekran 600px'den kucukse menuyu gizle */
  }
}
```

## 8\. HTML tablolarında satır ve sütunları birleştirmek için hangi etiketler kullanılır?

Cevap: `<td>` veya `<th>` etiketlerinde kullanilir. `colspan`: Sutun birlestirir. `colspan="2"` (iki sutunu birlestir). `rowspan`: Satir birlestirir. `rowspan="3"` (uc satiri birlestir).

## 9\. CSS ile bir butona hover efekti nasıl eklenir? Örnek kod yazınız.

Cevap: :hover sozde sinifi (pseudo-class) kullanilir. Fare ustune gelince calisir. Ornek:

```css
button {
  background-color: blue;
  color: white;
}
button:hover {
  background-color: darkblue; /* Fare gelince arkaplan koyulasir */
}
```

# Bölüm 3: Ağ Protokolleri ile İlgili Sorular

## 1\. HTTP ve HTTPS arasındaki temel farkları açıklayınız.

Cevap: HTTP duz metin gonderir. Guvenli degil. HTTPS (Secure) veriyi sifreler. SSL/TLS kullanir. Guvenlidir. HTTPS 443 portunu kullanir, HTTP 80 portunu.

## 2\. FTP nedir? Hangi amaçlarla kullanılır?

Cevap: FTP (File Transfer Protocol) dosya transfer protokolu. Sunucuya dosya yuklemek (upload) veya sunucudan dosya indirmek (download) icin kullanilir. Web sitesi dosyalari genelde FTP ile atilir.

## 3\. SMTP ve POP3 protokolleri arasındaki farkı açıklayınız.

Cevap: Ikisi de e-posta icin. SMTP (Simple Mail Transfer Protocol) e-posta gondermek icin kullanilir. POP3 (Post Office Protocol 3) e-postalari sunucudan cekmek (almak) icin kullanilir.

## 4\. DNS nedir? Çalışma mantığını kısaca anlatınız.

Cevap: DNS (Domain Name System) alan adi sistemi. https://www.google.com/search?q=google.com gibi isimleri 172.217.14.228 gibi IP adreslerine cevirir. Tarayiciya isim yazinca once DNS sunucusuna sorar, IP adresini ogrenir, sonra o IP’ye baglanir. Telefon rehberi gibi.

## 5\. DHCP protokolü ne işe yarar?

Cevap: DHCP (Dynamic Host Configuration Protocol) agdaki cihazlara otomatik IP adresi dagitir. Modeme baglaninca telefonun, bilgisayarin otomatik IP almasini saglar. Manuel IP ayarlamaya gerek kalmaz.

## 6\. HTTP 404 ve HTTP 500 hata kodları ne anlama gelir?

Cevap: 404 (Not Found): Istenen sayfa veya kaynak sunucuda bulunamadi. Yanlis link. Istemci hatasi. 500 (Internal Server Error): Sunucuda bir hata olustu. Kod patladi, veritabani baglanamadi falan. Sunucu hatasi.

## 7\. Telnet ve SSH arasındaki farkı açıklayınız.

Cevap: Ikisi de uzak sunucuya baglanip komut calistirmak icin. Telnet eski, guvensiz. Veriyi sifrelemez. SSH (Secure Shell) yeni, guvenli. Tum baglantiyi sifreler. Artik hep SSH kullanilir.

## 8\. VPN nedir ve hangi amaçlarla kullanılır?

Cevap: VPN (Virtual Private Network) sanal ozel ag. Internet baglantini sifreli bir tunel uzerinden yapar. Guvenlik saglar, kimligini gizler. Yasakli sitelere girmek veya sirket agina uzaktan guvenle baglanmak icin kullanilir.

## 9\. WebSockets nedir? Nasıl çalışır?

Cevap: WebSocket, tarayici ile sunucu arasinda cift yonlu, canli baglanti saglar. HTTP gibi surekli istek atmak gerekmez. Baglanti acilir, acik kalir. Sunucu istedigi an tarayiciya veri itebilir. Canli sohbet (chat) uygulamalari, anlik borsa verileri icin kullanilir.

## 10\. CDN (Content Delivery Network) nedir? Web sitelerinde nasıl kullanılır?

Cevap: CDN (Icerik Dagitim Agi) sitenin dosyalarini (resim, CSS, JS) dunyanin farkli yerlerindeki sunucularda kopyalar. Kullaniciya en yakin sunucudan dosyayi gonderir. Site cok hizli acilir.
