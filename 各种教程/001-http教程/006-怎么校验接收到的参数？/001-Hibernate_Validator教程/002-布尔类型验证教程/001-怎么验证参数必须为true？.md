# 怎么验证参数必须为true？



## 说明

- 对单一的参数进行验证，控制层需要添加@Validated
- 通过@AssertTrue注解验证



## 示例

```java
@RestController
@Validated
public class TestController {
    @GetMapping(value = "/hello")
    public String hello(@RequestParam(name = "b") @AssertTrue(message = "b必须为ture！") Boolean b) {
        return "b = " + b;
    }
}
```



## 测试

### 为false测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/02390cbd-50cc-4533-8a9d-2e486da02677694" alt="image.png" style="zoom:67%;" />



![image.png](http://81.71.143.136/figurebed/figurebedcontroller/picture/16680890-fe11-4c99-843d-2b8ea24aebc1695)



### 为true测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/7e410fcf-643b-487a-8d66-217ffa4e19e1696" alt="image.png" style="zoom:67%;" />





