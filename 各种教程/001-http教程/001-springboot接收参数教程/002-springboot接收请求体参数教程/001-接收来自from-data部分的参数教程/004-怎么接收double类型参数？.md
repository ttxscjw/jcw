# 怎么接收double类型参数？





## 说明

- 通过@RequestParam接收，通过value指定key



## 示例

```java
@PostMapping(value = "/hello")
    public String hello(@RequestParam(value = "double") double d) {
        return "double = " + d;
    }
```





## 测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/0e17949d-38cd-41eb-8c16-79c67bca240e679" alt="image.png" style="zoom:67%;" />