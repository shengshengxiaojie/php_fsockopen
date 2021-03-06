# fsockopen

[fsockopen](http://www.php.net/manual/zh/function.fsockopen.php) is socket package function, in addition to the basic commonly used TCP:// communication function, it also has other powerful communication function, UDP:// unix:// / udg:// and so on various protocols.

You can use  [stream_get_transports](http://php.net/manual/zh/function.stream-get-transports.php) to get the current server registered socket transfer protocol list to determine whether to support the need to use the agreement.

### Travis CI badge

[![Travis-ci](https://api.travis-ci.com/yakeing/php_fsockopen.svg)](https://travis-ci.com/yakeing/php_fsockopen)

### codecov badge

[![codecov](https://codecov.io/gh/yakeing/php_fsockopen/branch/master/graph/badge.svg)](https://codecov.io/gh/yakeing/php_fsockopen)

### Packagist badge

[![Version](http://img.shields.io/packagist/v/yakeing/php_fsockopen.svg)](../../releases)
[![Downloads](http://img.shields.io/packagist/dt/yakeing/php_fsockopen.svg)](https://packagist.org/packages/yakeing/php_fsockopen/dependents)

### Github badge

[![Downloads](https://img.shields.io/github/downloads/yakeing/php_fsockopen/total.svg)](../../)
[![Size](https://oauth.applinzi.com/Label/size/7.78KB/b36d41.svg)](src/fsockopen.php)
[![tag](https://oauth.applinzi.com/Label/tag/v2.1.0/28a745.svg)](../../releases)
[![license](https://oauth.applinzi.com/Label/license/MPL-2.0/FE7D37.svg)](LICENSE)
[![languages](https://oauth.applinzi.com/Label/languages/php/007EC6.svg)](../../search?l=php)

### Installation

Use [Composer](https://getcomposer.org) to install the library.
Of course, You can go to [Packagist](https://packagist.org/packages/yakeing/php_fsockopen) to view.

```
    $ composer require yakeing/php_fsockopen
```

### Initialization parameter

- [x] Sample：
```php
    $fs = new fsockopen();
    $ret = $fs->init(
        10, //Running time / sec (optional)
        tcp, //transport protocol (optional)
        true //Blocking mode switch (optional)
        );
```

### Get network resources

- [x] Sample：
```php
    $ret = $fs->GET(
        $Url , //Destination URL
        $Referer , //Forge Referer (optional)
        $Cookie //This Cookie (optional)
    );
```


### POST Submit Form

- [x] Sample：
```php
    $ret = $fs->POST(
        $Url , //Destination URL
        $Content , //Submit content: key/vvalue&...
        $Referer , //Forge Referer (optional)
        $Cookie, //This Cookie (optional)
        $ContentType //Submission method (optional)
    );
```

### POST File

- [x] Sample：
```php
    $ret = $fs->PUT(
        $Url , //Destination URL
        $File, //File OR Picture address: ['01.jpg','02.jpg',...]
        $Referer , //Forge Referer (optional)
        $Cookie, //This Cookie (optional)
    );
```

[Sponsor](https://github.com/yakeing/Documentation/blob/master/Sponsor/README.md)
---
If you've got value from any of the content which I have created, then I would very much appreciate your support by payment donate.

[![Sponsor](https://oauth.applinzi.com/State/heart/Sponsor/EA4AAA.svg)](https://github.com/yakeing/Documentation/blob/master/Sponsor/README.md)

Author
---

weibo: [yakeing](https://weibo.com/yakeing)

twitter: [yakeing](https://twitter.com/yakeing)
