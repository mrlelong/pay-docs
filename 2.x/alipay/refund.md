# 退款 - Wechat

| 方法名 | 参数 | 返回值 |
| :---: | :---: | :---: |
| refund | array $order | Collection |

---

- [退款操作](#退款操作)
- [配置参数](#配置参数)
- [返回值](#返回值)

<a name="退款操作"></a>

## 退款操作

```PHP
$order = [
    'out_trade_no' => '1514027114',
    'refund_amount' => '0.01',
];

$result = $alipay->refund($order);
```


<a name="配置参数"></a>

## 配置参数

所有订单配置参数和官方无任何差别，兼容所有功能，所有参数请参考[这里](https://docs.open.alipay.com/api_1/alipay.trade.refund)，查看「请求参数」一栏。


<a name="返回值"></a>

## 返回值

返回 Collection 类型，可以通过 `$collection->xxx` 得到服务器返回的数据。
