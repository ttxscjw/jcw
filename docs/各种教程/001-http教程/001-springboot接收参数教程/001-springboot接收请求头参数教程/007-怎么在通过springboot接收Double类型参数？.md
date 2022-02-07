# 怎么在通过springboot接收Double类型参数？





## 说明

- 通过@RequestParam注解接收
- 可以被直接接收



## 示例

```java
@GetMapping(value = "/hello")
    public String hello(@RequestParam(name = "Double") Double d) {
        return "Double = " + d;
    }
```





## 测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/0a39ad5e-1f48-449f-978f-88466c4c164c658" alt="image.png" style="zoom:67%;" />



