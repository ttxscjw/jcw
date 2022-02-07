# http怎么通过url发送参数？



## 示例

```http
http://localhost:8080/hello/?name=cjw&age=13&num=1
```



- 以？开始
- key=value格式
- 以&分割参数



## 在springboot中接收



```java
/**
     * @title
     * @description
     * @author admin cjw
     * @updateTime 2021/10/8 15:14
     */
    @GetMapping(value = "/hello")
    public String hello(@RequestParam(name = "name") String name, @RequestParam(name = "age") Integer age,
                        @RequestParam(name = "num") int num) {
        return "name="+name+",age="+age+",num="+num;
    }
```





## 测试

- 使用postman



<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/d2da1521-03ae-4e86-97d4-d3c67522eb5d651" alt="image.png" style="zoom:50%;" />