# springboot

- 更快捷的整合第三方框架
- 内嵌服务器（tomcat、jetty、undertow）
- 使用注解代替 xml



### 注解

**RestController**

    定义当前类所有方法的返回统一为 json 格式数据
    该注解整合类 spring 的 @Controller + @ResponseBody 

**EnableAutoConfiguration**

    快速启动 web 服务，内嵌服务器（tomcat等服务器）
    该包扫描范围为当前类


**RequestMapping**

    定义 url 路径

**ComponentScan**

    定义那些包需要被扫描