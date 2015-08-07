Telegram bot API for Yii2
================
[![Packagist](https://img.shields.io/packagist/l/sonko-dmitry/botan-php-sdk.svg)](https://github.com/SonkoDmitry/botan-php-sdk/blob/master/LICENSE.md)
[![Packagist](https://img.shields.io/packagist/v/sonko-dmitry/botan-php-sdk.svg)](https://packagist.org/packages/sonko-dmitry/botan-php-sdk)
[![Packagist](https://img.shields.io/packagist/dt/sonko-dmitry/botan-php-sdk.svg)](https://packagist.org/packages/sonko-dmitry/botan-php-sdk)
This extension is the way to integrate [Botan.io](http://botan.io/) to you application.

Installation
------------
The preferred way to install this extension is through [composer](http://getcomposer.org/download/). 

 To install, either run
 ```
 $ php composer.phar require sonko-dmitry/botan-php-sdk:*
 ```
 or add
 ```
 "sonko-dmitry/botan-php-sdk": "*"
 ```
 to the `require` section of your `composer.json` file.


Usage
-----
0. Now you can use wrapper
 ```php
 $tracker = new SonkoDmitry\BotanSDK\BotanTracker(1234567);
 $tracker->track(123, ['text' => 'Hello world!'], 'Message');
 ```
 Where "1234567" your [Yandex.Appmetrica](https://appmetrika.yandex.com/) api token. 123 unique customer ID, for example chat_id or sender_id