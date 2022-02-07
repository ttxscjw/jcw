# 怎么接收json数组转自动转list？





## 说明

- 通过@RequestBody接收
- list需要指定泛型



## 示例

```java
@PostMapping(value = "/hello")
    public String hello(@RequestBody List<String> list) {
        return "List = " + list;
    }
```





## 测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/78d8c108-2d5c-42fb-891d-a458ebca1ee8686" alt="image.png" style="zoom:67%;" />