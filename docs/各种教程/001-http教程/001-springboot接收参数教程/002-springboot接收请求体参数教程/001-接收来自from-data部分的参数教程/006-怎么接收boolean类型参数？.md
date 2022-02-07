# 怎么接收boolean类型参数？





## 说明

- 通过@RequestParam接收，通过value指定key



## 示例

```java
@PostMapping(value = "/hello")
    public String hello(@RequestParam(value = "boolean") boolean b) {
        return "boolean = " + b;
    }
```





## 测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/2f81fdde-43de-46d5-a4a9-83cf20c85bc3680" alt="image.png" style="zoom:67%;" />