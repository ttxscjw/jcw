# 怎么接收string类型参数？





## 说明

- 通过@RequestParam接收，通过value指定key



## 示例

```java
@PostMapping(value = "/hello")
    public String hello(@RequestParam(value = "name") String name) {
        return "name = " + name;
    }
```





## 测试

<img src="http://81.71.143.136/figurebed/figurebedcontroller/picture/fcba944c-98f3-4930-ae5b-d4bbce7c5000676" alt="image.png" style="zoom:67%;" />