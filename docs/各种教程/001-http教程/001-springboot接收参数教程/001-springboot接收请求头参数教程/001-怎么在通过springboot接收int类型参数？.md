# 怎么在通过springboot接收int类型参数？





## 说明

- 通过@RequestParam注解接收



## 示例

```java
@GetMapping(value = "/hello")
    public String hello(@RequestParam(name = "num") int num) {
        return "num = " + num;
    }
```





## 测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/b0f7440d-9d15-4f69-aeba-8e981985896e652" alt="image.png" style="zoom:50%;" />



