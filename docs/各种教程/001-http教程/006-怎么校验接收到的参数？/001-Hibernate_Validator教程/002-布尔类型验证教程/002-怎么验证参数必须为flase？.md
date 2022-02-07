# 怎么验证参数必须为flase



## 说明

- 对单一的参数进行验证，控制层需要添加@Validated
- 通过@AssertFalse注解验证



## 示例

```java
@RestController
@Validated
public class TestController {
    @GetMapping(value = "/hello")
    public String hello(@RequestParam(name = "b") @AssertFalse(message = "b必须为false！") Boolean b) {
        return "b = " + b;
    }
}
```



## 测试

### 为false测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/ae42774f-71c1-451c-bfa6-dc57b4f39a9b699" alt="image.png" style="zoom:67%;" />







### 为true测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/2e898ba4-a255-4776-bf38-e7f4b052a7e0697" alt="image.png" style="zoom: 67%;" />



![image.png](http://81.71.143.136/figurebed/figurebedcontroller/picture/a9630f2e-1050-4362-aea4-ca911e773f74698)

