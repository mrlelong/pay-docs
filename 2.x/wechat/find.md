# 查询 - Wechat

| 方法名 | 参数 | 返回值 |
| :---: | :---: | :---: |
| find | string/array $order, string/null $type | Collection |

---

- [查询普通支付订单](#查询普通支付订单)
- [查询退款订单](#查询退款订单)
- [查询企业付款订单](#查询企业付款订单)
- [订单配置参数](#订单配置参数)
- [返回值](#返回值)

<a name="查询普通支付订单"></a>

## 查询普通支付订单

```PHP
$order = [
    'out_trade_no' => '1514027114',
];
// $order = '1514027114';

$result = $wechat->find($order);
```

<a name="查询退款订单"></a>

## 查询退款订单

```PHP
$order = [
    'out_trade_no' => '1514027114',
];
// $order = '1514027114';

$result = $wechat->find($order, 'refund');
```

<a name="查询企业付款订单"></a>

## 查询企业付款订单

> {info} v2.7.8 及以上可用

```PHP
$order = [
    'partner_trade_no' => '1514027114',
];
// $order = '1514027114';

$result = $wechat->find($order, 'transfer');
```

<a name="订单配置参数"></a>

## 订单配置参数

### 查询订单

所有订单配置参数和官方无任何差别，兼容所有功能，所有参数请参考[这里](https://pay.weixin.qq.com/wiki/doc/api/jsapi.php?chapter=9_2)，查看「请求参数」一栏。

### 查询退款订单

所有订单配置参数和官方无任何差别，兼容所有功能，所有参数请参考[这里](https://pay.weixin.qq.com/wiki/doc/api/jsapi.php?chapter=9_5)，查看「请求参数」一栏。

### 查询企业付款订单

所有订单配置参数和官方无任何差别，兼容所有功能，所有参数请参考[这里](https://pay.weixin.qq.com/wiki/doc/api/tools/mch_pay.php?chapter=14_3)，查看「请求参数」一栏。

### APP/小程序查询

如果您需要查询 `APP/小程序` 的订单，请传入参数：`['type' => 'app']`/`['type' => 'miniapp']`

<a name="返回值"></a>

## 返回值

返回 Collection 类型，可以通过 `$collection->xxx` 得到服务器返回的数据。
