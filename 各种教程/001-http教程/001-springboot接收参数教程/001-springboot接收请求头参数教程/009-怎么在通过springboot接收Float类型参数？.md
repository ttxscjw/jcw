# 怎么在通过springboot接收Float类型参数？





## 说明

- 通过@RequestParam注解接收
- 可以被直接接收



## 示例

```java
@GetMapping(value = "/hello")
    public String hello(@RequestParam(name = "Float") Float f) {
        return "Float = " + f;
    }
```





## 测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/8e27b254-6cfe-4001-a6f3-beace596581d660" alt="image.png" style="zoom:67%;" />



