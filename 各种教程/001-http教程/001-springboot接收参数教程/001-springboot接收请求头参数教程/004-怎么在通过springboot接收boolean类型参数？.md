# 怎么在通过springboot接收boolean类型参数？





## 说明

- 通过@RequestParam注解接收
- 可以被直接接收



## 示例

```java
@GetMapping(value = "/hello")
    public String hello(@RequestParam(name = "b") boolean b) {
        return "boolean = " + b;
    }
```





## 测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/9a89993b-6259-455a-9311-cee83e9f7058656" alt="image.png" style="zoom:67%;" />



