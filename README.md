Magento-URLs
============

A Resource Of Magento URL's

```php

To Retrieve URL path in STATIC BLOCK
---------------------------------------
To get SKIN URL
{{skin url='images/sampleimage.jpg'}}
 
To get Media URL
{{media url='/sampleimage.jpg'}}
 
To get Store URL
{{store url='mypage.html'}}
 
To get Base URL
{{base url='yourstore/mypage.html'}}
 
 
TO Retrieve URL path in PHTML
---------------------------------------
 
Not secure Skin URL:
<?php echo $this->getSkinUrl('images/sampleimage.jpg') ?>
 
Secure Skin URL
<?php echo $this->getSkinUrl('images/ sampleimage.gif', array('_secure'=>true)) ?>
 
Get  Current URL
$current_url = Mage::helper('core/url')->getCurrentUrl();
 
Get Home URL
$home_url = Mage::helper('core/url')->getHomeUrl();
 
Get Magento Media Url
Mage::getBaseUrl(Mage_Core_Model_Store::URL_TYPE_LINK);
 
Get Magento Media Url
Mage::getBaseUrl(Mage_Core_Model_Store::URL_TYPE_MEDIA);
 
Get Magento Skin Url
Mage::getBaseUrl(Mage_Core_Model_Store::URL_TYPE_SKIN);
 
Get Magento Store Url
Mage::getBaseUrl(Mage_Core_Model_Store::URL_TYPE_WEB);
 
Get Magento Js Url
Mage::getBaseUrl(Mage_Core_Model_Store::URL_TYPE_JS);



Mage::getBaseUrl() => Gets base url path e.g. http://my.website.com/

Mage::getBaseUrl('media') => Gets MEDIA folder path e.g. http://my.website.com/media/

Mage::getBaseUrl('js') => Gets JS folder path e.g. http://my.website.com/js/

Mage::getBaseUrl('skin') => Gets SKIN folder path e.g. http://my.website.com/skin/

Get DIRECTORY paths (physical location of your folders on the server) – Relative URL Path

Mage::getBaseDir() => Gives you your Magento installation folder / root folder e.g. /home/kalpesh/workspace/magento

Mage::getBaseDir('app') => Gives you your Magento's APP directory file location e.g. /home/kalpesh/workspace/magento/app

Mage::getBaseDir('design') => Gives you your Magento's DESIGN directory file location e.g. /home/kalpesh/workspace/magento/design

Mage::getBaseDir('media') => Gives MEDIA directory file path

Mage::getBaseDir('code') => Gives CODE directory file path

Mage::getBaseDir('lib') => Gives LIB directory file path

Mage::helper('core/url')->getCurrentUrl()

base Mage::getBaseDir()

Mage::getBaseDir('base') /var/www/magento/

app Mage::getBaseDir('app') /var/www/magento/app/

code Mage::getBaseDir('code') /var/www/magento/app/code

design Mage::getBaseDir('design') /var/www/magento/app/design/

etc Mage::getBaseDir('etc') /var/www/magento/app/etc

lib Mage::getBaseDir('lib') /var/www/magento/lib

locale Mage::getBaseDir('locale') /var/www/magento/app/locale

media Mage::getBaseDir('media') /var/www/magento/media/

skin Mage::getBaseDir('skin') /var/www/magento/skin/

var Mage::getBaseDir('var') /var/www/magento/var/

tmp Mage::getBaseDir('tmp') /var/www/magento/var/tmp

cache Mage::getBaseDir('cache') /var/www/magento/var/cache

log Mage::getBaseDir('log') /var/www/magento/var/log

session Mage::getBaseDir('session') /var/www/magento/var/session

upload Mage::getBaseDir('upload') /var/www/magento/media/upload

export Mage::getBaseDir('export') /var/www/magento/var/export
```
