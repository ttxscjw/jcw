# 怎么接收Date类型参数？





## 说明

- 通过@RequestParam接收，通过value指定key
- 通过@DateTimeFormat指定解析的格式



## 示例

```java
@PostMapping(value = "/hello")
    public String hello(@RequestParam(name = "date") @DateTimeFormat(pattern = "yyyy-MM-dd HH:mm:ss")  Date date) {
        SimpleDateFormat dateFormat = new SimpleDateFormat("yyyy-MM-dd HH:mm:ss");
        String format = dateFormat.format(date);
        return "Date = " + format;
    }
```





## 测试

![image.png](http://81.71.143.136/figurebed/figurebedcontroller/picture/6534d783-9e6a-4c1e-984d-c59f5efbc569682)