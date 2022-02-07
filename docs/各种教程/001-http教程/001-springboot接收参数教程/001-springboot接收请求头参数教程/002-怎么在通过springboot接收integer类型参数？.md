# 怎么在通过springboot接收integer类型参数





## 说明

- 通过@RequestParam注解接收
- 可以被直接接收



## 示例

```java
@GetMapping(value = "/hello")
    public String hello(@RequestParam(name = "integer") Integer integer) {
        return "Integer = " + integer;
    }
```





## 测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/5364f546-3266-4420-958b-603cf2a513d5653" alt="image.png" style="zoom: 67%;" />



