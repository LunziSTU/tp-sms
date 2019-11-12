# tp-sms

thinkphp6 短信验证码生成、验证类库

## 安装
> composer require lunzi/tp-sms


## 使用

### 生成验证码

~~~
use lunzi\TpSms;

$tpSms = new TpSms();
$code = $tpSms->create();
~~~

### 验证

~~~
if(!$tpSms->check()){
    //验证失败，获取失败信息
    $msg = $tpSms->getErrorMsg();
};
~~~
