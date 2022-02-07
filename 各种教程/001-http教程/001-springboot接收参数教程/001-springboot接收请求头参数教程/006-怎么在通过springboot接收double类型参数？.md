# 怎么在通过springboot接收double类型参数?





## 说明

- 通过@RequestParam注解接收
- 可以被直接接收



## 示例

```java
@GetMapping(value = "/hello")
    public String hello(@RequestParam(name = "double") double d) {
        return "double = " + d;
    }
```





## 测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/08c44d9f-3466-4f54-95b0-947c917757a7657" alt="image.png" style="zoom:67%;" />



