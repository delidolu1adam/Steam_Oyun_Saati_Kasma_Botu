# GELİŞTİRİCİ NOTU: Bu proje askıya alınmış olarak kabul edilebilir. Muhtemelen başka bir dilde daha iyi kod ve daha fazla özellik içeren tamamen yeni bir proje oluşturacağım.

# Steam Oyun Saati Artırıcı, 2FA desteğine sahip bilgisayarınızda veya sunucuda çalıştırabileceğiniz basit bir Steam saat artırma botu'dur.

Bu [**NodeJS**](https://nodejs.org/en/download/) betiğiyle 2FA desteğiyle, aynı anda birden fazla steam hesabının oyun saatlerini artırın!  
_(Ve paylaşılabilir gizli anahtarı kullanmak gerekli değildir)_

## Nasıl kurulur?

```bash
# Bağımlılıkları yükleyin ⌨️
$ npm install
```

## Nasıl çalıştırılır?

```bash
# Botu başlatın 🎉
$ npm run start
```

## config/accounts.js dosyasındaki yapılandırma örneği

```javascript
var configsArray = []; // Bu kodu değiştirmeyin veya silmeyin!
var config; // Bu kodu değiştirmeyin veya silmeyin!

// Account 1
config = {};
config.username = 'Hesap_Adınız';
config.password = 'Hesap_Parolanız';
config.sharedSecret = '';
config.enableStatus = true;
config.gamesAndStatus = ['Half-Life 3', 10, 70, 240, 440, 570, 730, 218230, 252490, 578080, 1085660, 1172470, 1962663, 552990,];
config.replyMessage = 'Steam oyun saatlerimi arttırmak için boşta bekliyorum.';
config.receiveMessages = false;
config.saveMessages = false;
configsArray.push(config);

module.exports = configsArray; // Bu kodu değiştirmeyin veya silmeyin!
```
