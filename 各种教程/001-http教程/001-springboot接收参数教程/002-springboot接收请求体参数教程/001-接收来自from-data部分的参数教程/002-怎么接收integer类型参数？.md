# 怎么接收integer类型参数？





## 说明

- 通过@RequestParam接收，通过value指定key



## 示例

```java
@PostMapping(value = "/hello")
    public String hello(@RequestParam(value = "integer") Integer integer) {
        return "Integer = " + integer;
    }
```





## 测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/8c0fceda-2d8a-412f-a86f-b84bf81f84d9675" alt="image.png" style="zoom:67%;" />