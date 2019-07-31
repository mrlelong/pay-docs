## 验证服务器数据 - Wechat

| 方法名 | 参数 | 返回值 |
| :---: | :---: | :---: |
| verify | 无 | Collection |

---

- [支付异步通知验证](#支付异步通知验证)
- [退款异步通知验证](#退款异步通知验证)
- [配置参数](#配置参数)
- [返回值](#返回值)

<a name="支付异步通知验证"></a>

## 支付异步通知验证

```PHP
$result = $wechat->verify();
// 是的，你没有看错，就是这么简单！

// return $wechat->success()->send(); // laravel 框架直接 return $wechat->success();
```

<a name="退款异步通知验证"></a>

## 退款异步通知验证

> {info} v2.4.0 及以上可用

```PHP
$result = $wechat->verify(null, true);
// 是的，你没有看错，就是这么简单！

// return $wechat->success()->send(); // laravel 框架直接 return $wechat->success();
```

<a name="配置参数"></a>

## 配置参数

无

<a name="返回值"></a>

## 返回值

返回 Collection 类型，可以通过 `$collection->xxx` 得到服务器返回的数据。
