# 怎么在通过springboot接收Boolean类型参数？





## 说明

- 通过@RequestParam注解接收
- 可以被直接接收



## 示例

```java
@GetMapping(value = "/hello")
    public String hello(@RequestParam(name = "b") Boolean b) {
        return "b = " + b;
    }
```





## 测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/5a95ddc0-cee3-4e94-a4b2-307505113cee655" alt="image.png" style="zoom:67%;" />



