# 怎么接收自定义对象？







## 说明

- 使用@RequestBody接收



## 示例

```java
@RestController
public class TestController {
    @PostMapping(value = "/hello")
    public String hello(@RequestBody  People people) {
        return "people = " + people;
    }
}
```





## 测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/ea74ac69-ca96-4be1-b69f-df5b7bdd0619731" alt="image.png" style="zoom:67%;" />