#医疗系统框架说明

--- 

> ###项目结构说明：

- java  cn.stylefeng.guns 所有实现类与业务代码和工具类的合集

    #### 主包功能说明:
    
   
   
        * config.datasource 单数据源与多数据源配置相关内容（包含mybatis部分插件）
        
        * config.properties beels与项目相关配置
        
        * config.web 缓存，在线接口文档相关配置

        * config.core springboot整合核心配置 
            实现aop切面编程，Aop拦截器，监听器，日志，登陆验证，以及部分工具类等。
        
        * config.modular conyroller与service层的结合体，每层功能单独模块化
            包含mapper和mapper.xml文件与启动类

    

- resource 配置文件
 
      TODO 项目主干配置文件 
     #### 类库功能说明:
       
      application.yml:
        
        * server:port 服务启动端口配置
        * guns:  项目swagger与登陆验证配置开关等
        * beetl： 热加载beetl模板  
        * spring： spirng框架配置
        * log： 日志配置
        * 等等.... 
        
      ehcache.xml：
      
        * 缓存配置xml文件
        
      logback-spring.xml:
        
        * 日志配置xml文件
       
- webapp 静态文件与前端页面

     static：静态文件

        css， 引用外部样式css文件

        fonts，引用字体文件
        
        img，项目中使用的图片文件夹
        
        js，引用的外部js文件
        
        modular，项目核心js相关文件
        
     WEB-INF：前端html页面

        req类， 业务相关请求对象类。

        resp类， 业务相关返回对象类。
    

- test 编写测试类
        
        仅供测试使用，内涵项目主导工具类以及相关加密测试，
        建议在使用此项目之前首先了解相关测试。
        
    
#### 其他
项目构建使用了spring2.0版本，单体服务应用，
使用mysql数据库，IDEA开发工具，
运行sql脚本之后，可直接运行。
    
