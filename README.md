# Bot Hakkında
Steam Oyun Saati Artırıcı, 2FA desteğine sahip "kişisel bilgisayarınızda" veya "sunucuda" çalıştırabileceğiniz basit ve güvenli bir Steam saat artırma botu'dur.

# Geliştirici Notu
Bu proje askıya alınmış olarak kabul edilebilir. Muhtemelen başka bir dilde daha iyi kod ve daha fazla özellik içeren tamamen yeni bir proje oluşturacağım.

## NodeJS'yi yükleyin
İlk olarak [**NodeJS**](https://nodejs.org/tr/download/)'nin son sürümünü resmi web sitesinden indirin ve bilgisayarınıza kurun. 

## Bağlılıkları yükleyin
```bash
$ npm install
```
## Popüler oyun kimlikleri
```bash
10 = Counter-Strike
70 = Half-Life
80 = Counter-Strike Zero
220 = Half-Life 2
240 = Counter-Strike: Source
440 = Team Fortress 2
570 = Dota 2
730 = Counter-Strike 2
218230 = PlanetSide 2
252490 = Rust
578080 = PUBG
1063730 = New World
1085660 = Destiny 2
1172470 = Apex Legend
1517290 = Battlefield™ 2042
1962663 = C.O.D Warzone
2073850 = The Finals
```

## Oyun kimliğini nasıl öğrenebilirim?
```bash
1: Steam mağaza sayfasını açın.
2: Arama kutusuna Rust yazın ve oyun sayfasını açın.
3: Açılan sayfada adres çubuğundaki URL şu şekilde olmalıdır: https://store.steampowered.com/app/252490/Rust/
4: URL içindeki bu "252490" numaralar oyunun benzersiz steam kimliğidir.
```

## Örnek config/accounts.js yapılandırması
```javascript
// Bu kodları değiştirmeyin veya silmeyin!
var configsArray = []; 
var config;

// Steam Hesabı 1
config = {};
// Steam hesap adı
config.username = 'Hesap_Adınız';
// Steam hesap parolası
config.password = 'Hesap_Parolanız';
// Steam Guard kodu kullanacaksanız burayı boş bırakın.
config.sharedSecret = '';
// Çevrimiçi durumunuzu görünmez kılmak için bu değeri "false" olarak değiştirin.
config.enableStatus = true;
// Steam profilinizde görünmesini istediğiniz özel mesaj ve oyunların Steam mağazası kimlikleri.
config.gamesAndStatus = ['Half-Life 3', 10, 70, 240, 440, 570, 730, 218230, 252490, 578080, 1085660, 1172470, 1962663, 552990,];
// Arkadaş listenizden birisi size mesaj gönderdiğinde otomatik yanıtlayın.
config.replyMessage = 'Steam oyun saatlerimi arttırmak için boşta bekliyorum.';
// Komut terminali mesajlarını bir dosyaya kaydetmek istiyorsanız bu değeri "true" olarak değiştirin.
config.receiveMessages = false;
// Sohbet mesajlarını bir dosyaya kaydetmek istiyorsanız bu değeri "true" olarak değiştirin.
config.saveMessages = false;
// Bu kodu değiştirmeyin veya silmeyin!
configsArray.push(config);

// Bu kodu değiştirmeyin veya silmeyin!
module.exports = configsArray;
```

## Botu çalıştırın
```bash
$ npm run start
```



