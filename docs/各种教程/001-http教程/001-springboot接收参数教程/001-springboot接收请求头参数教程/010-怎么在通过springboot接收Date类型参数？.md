# 怎么接收Date类型参数？





## 说明

- 通过@RequestParam接收，通过value指定key
- 通过@DateTimeFormat指定解析的格式



## 示例

```java
@GetMapping(value = "/hello")
    public String hello(@RequestParam(name = "date") @DateTimeFormat(pattern = "yyyy-MM-dd HH:mm:ss")  Date date) {
        SimpleDateFormat dateFormat = new SimpleDateFormat("yyyy-MM-dd HH:mm:ss");
        String format = dateFormat.format(date);
        return "Date = " + format;
    }
```





## 测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/1d8cb8ed-f2e7-4ba3-8336-ef092b910fe5683" alt="image.png" style="zoom:67%;" />