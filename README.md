# vk-php-sdk with proxy

## 1. Changes regarding the official package

* Proxy support added
* Method execute() for executing VKScript code

## 2. Prerequisites

* PHP 7.1 or later

## 3. Installation

add to composer.json:

```json
    "repositories":
    [
      {
        "type": "vcs",
        "url": "https://github.com/takoyta/vk-proxy"
      }
    ],
    ...
    "require": {
      "takoyta/vk-proxy": "dev-master"
```

## 4. Initialization

Create VKApiClient object using the following code:

```php
$vk = new VK\Client\VKApiClient();
$vk->setProxy('127.0.0.1:8080', CURLPROXY_HTTP);
```

