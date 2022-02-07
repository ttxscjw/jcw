# 怎么接收json对象转自动转map？





## 说明

- 通过@RequestBody接收



## 示例

```java
@PostMapping(value = "/hello")
    public String hello(@RequestBody Map map) {
        return "Map = " + map;
    }
```





## 测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/81bd54b4-96ef-4e6a-b2e4-0e9a8f6421bf685" alt="image.png" style="zoom:67%;" />