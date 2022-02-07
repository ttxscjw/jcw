# 怎么在通过springboot接收string类型参数？





## 说明

- 通过@RequestParam注解接收
- 可以被直接接收



## 示例

```java
@GetMapping(value = "/hello")
    public String hello(@RequestParam(name = "s") String s) {
        return "s = " + s;
    }
```





## 测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/b7acf1c2-901a-45e4-b3e5-70c1d6f5f775654" alt="image.png" style="zoom: 67%;" />



