# Google Authenticator PHP 



## CONTATO 
 
<p>
<a href="https://wa.me/5566996852025" target="_blank"> 
 <img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" title="+55 66 99685-2025"/> 
</a>

 <a href="https://t.me/raphaelserafim" target="_blank">
  <img src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" target="_blank">
 </a>  

<a href="https://instagram.com/raphaelvserafim" target="_blank">
 <img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank">
</a>
 
<a href="https://www.linkedin.com/in/raphaelvserafim" target="_blank">
 <img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank">
</a>  
</p>
 

## Example of use:

```php
use Cachesistemas\GoogleAuthenticator;

include_once 'vendor/autoload.php';

$ga  = new GoogleAuthenticator():
```

### create Secret
```php
$secret = $ga->createSecret();
```

### get QRCode Google Url
```php
$qrCode = $ga->getQRCodeGoogleUrl("<email>", $secret,"<NAME>");
```

### verify Code
```php
$check = $ga->verifyCode($secret, "<code>", 2);
```

