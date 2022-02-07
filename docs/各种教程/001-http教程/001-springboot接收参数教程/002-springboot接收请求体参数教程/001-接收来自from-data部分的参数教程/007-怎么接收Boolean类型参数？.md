# 怎么接收Boolean类型参数？





## 说明

- 通过@RequestParam接收，通过value指定key



## 示例

```java
@PostMapping(value = "/hello")
    public String hello(@RequestParam(value = "Boolean") Boolean b) {
        return "Boolean = " + b;
    }

```





## 测试

![image.png](http://81.71.143.136/figurebed/figurebedcontroller/picture/4d3cbf2d-b5a3-4af6-bcb1-ce013929ebdd681)