# 关闭 - Alipay

| 方法名 | 参数 | 返回值 |
| :---: | :---: | :---: |
| close | string/array $order | Collection |

---

- [例子](#例子)
- [配置参数](#配置参数)
- [返回值](#返回值)


<a name="例子"></a>

## 例子

```PHP
$order = [
    'out_trade_no' => '1514027114',
];

// $order = '1514027114';

$result = $alipay->close($order);
```


<a name="配置参数"></a>

## 配置参数

所有订单配置参数和官方无任何差别，兼容所有功能，所有参数请参考[这里](https://docs.open.alipay.com/api_1/alipay.trade.close/)，查看「请求参数」一栏。


<a name="返回值"></a>

## 返回值

返回 Collection 类型，可以通过 `$collection->xxx` 得到服务器返回的数据。
