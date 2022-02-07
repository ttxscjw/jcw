# 怎么接收Double类型参数？





## 说明

- 通过@RequestParam接收，通过value指定key



## 示例

```java
@PostMapping(value = "/hello")
    public String hello(@RequestParam(value = "Double") Double d) {
        return "Double = " + d;
    }
```





## 测试

![image.png](http://81.71.143.136/figurebed/figurebedcontroller/picture/6362e084-3903-4450-ac74-f5e7cf5d1a20678)