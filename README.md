根据指纹判断cms系统
==========

PHP Library for detecting CMS

Install
-------

```bash
composer require "adzon/php-cms-detector"
```

How to use:
-----------

    $domain = "http://google.com";
    $cms = new \DetectCMS\DetectCMS($domain);
    if($cms->getResult()) {
        echo "Detected CMS: ".$cms->getResult();
    } else {
        echo "CMS couldn't be detected";
    } 