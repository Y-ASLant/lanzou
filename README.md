# lanzou API

#### 介绍
蓝奏云盘 直链解析API
#### 支持的功能
- 检测文件是否被取消

- 带密码的文件分享链接但不支持分享的文件夹

- 生成直链或直接下载


#### 使用说明

url:蓝奏云外链链接

type:是否直接下载 值：down

pwd:外链密码

内部调用方法

```php
include('lanzou.clsss.php');
$lz = new lanzou;
$res=$lz->getUrl($url,$pwd);
```

# 使用示例

直接下载：
无密码：http://tool.bitefu.net/lanzou/?url=https://www.lanzous.com/xxxx&type=down

有密码：http://tool.bitefu.net/lanzou/?url=https://www.lanzous.com/xxxxx&type=down&pwd=1234

输出直链：
无密码：http://tool.bitefu.net/lanzou/?url=https://www.lanzous.com/xxxxx

有密码：http://tool.bitefu.net/lanzou/?url=https://www.lanzous.com/xxxx&pwd=1234

#### 短链接

不带密码:http://tool.bitefu.net/lanzou/?d=iXAYR0e10dpe

带密码:http://tool.bitefu.net/lanzou/?d=ic3qfri-52pj
