# 说明

| 方法名 | 参数 | 返回值 |
| :---: | :---: | :---: |
| success | 无 | Response |

---

- [例子](#例子)
- [配置参数](#配置参数)
- [返回值](#返回值)


<a name="例子"></a>

## 例子

```PHP
// $result = $alipay->verify();

return $alipay->success()->send(); // laravel 框架直接 return $alipay->success();
```

<a name="配置参数"></a>

## 订单配置参数

无

<a name="返回值"></a>

## 返回值

返回 Response 类型，可以通过`return $response->send();` 进行返回；如果在 laravel 框架中，可直接 `return $response;`
