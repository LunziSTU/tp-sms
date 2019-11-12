# tp-sms

适用于 thinkphp6 的短信验证码生成、验证类库

## 主要特性
* 支持 7 种验证码类型
* 基于 ThinkPHP 缓存
* 灵活的配置机制

## 安装
~~~php
composer require lunzi/tp-sms
~~~

## 使用示例

### 生成验证码

~~~php
use lunzi\TpSms;

$tpSms = new TpSms();
$code = $tpSms->create();
~~~

### 验证

~~~php
if(!$tpSms->check()){
    //验证失败，获取失败信息
    $msg = $tpSms->getErrorMsg();
};
~~~

## 版权信息
TpSms遵循Apache2开源协议发布，并提供免费使用。