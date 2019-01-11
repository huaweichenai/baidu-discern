# 百度实现图片识别文本包


[![Latest Stable Version](https://poser.pugx.org/huaweichenai/baidu-discern/v/stable)](https://packagist.org/packages/huaweichenai/baidu-discern) 
[![Total Downloads](https://poser.pugx.org/huaweichenai/baidu-discern/downloads)](https://packagist.org/packages/huaweichenai/baidu-discern) 
[![Latest Unstable Version](https://poser.pugx.org/huaweichenai/baidu-discern/v/unstable)](https://packagist.org/packages/huaweichenai/baidu-discern) 
[![License](https://poser.pugx.org/huaweichenai/baidu-discern/license)](https://packagist.org/packages/huaweichenai/baidu-discern)


## Installation<br>
```
composer require huaweichenai/baidu-discern<br>
```
## Usage<br>
### Configuration:
配置文件添加组件 :<br>
```
'aipImg' => [<br>
            'class' => 'huaweichenai\discern\AipOcr',
            'appId' => '百度文字App ID',
            'apiKey' => '百度文字 API Key',
            'secretKey' => '百度文字 Secret Key',
        ],
```
### use:<br>
```
$client = Yii::$app->aipImg;
$image = file_get_contents('图片地址');
$content = $client->basicAccurate($image);
```
