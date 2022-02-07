# 怎么在通过springboot接收float类型参数？





## 说明

- 通过@RequestParam注解接收
- 可以被直接接收



## 示例

```java
@GetMapping(value = "/hello")
    public String hello(@RequestParam(name = "float") float f) {
        return "float = " + f;
    }
```





## 测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/b80dbf23-ed4c-4005-9f3a-acab6b003058659" alt="image.png" style="zoom:67%;" />



