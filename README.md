# user_center  
用户中心  
=
项目介绍  
基于Spring Boot+React的一站式用户管理系统，实现了用户注册、登泉、查询管理等功能。  
主要工作  
1.选用MyBatis+MyBatis-Plus进行数据访问层开发，复用大多数通用方法，并且通过继承定制了自己的通用操作模板，大幅提升了项目开发效率。  
2.为了明确接口的返回，自定义统一的错误码，并封装了全局异常处理器，从而规范了异常返回、屏蔽了项目冗余的报错细节。  
3.对于项目中的SON格式化处理对象，采用双检锁单例模式进行管理，从而复用对象，避免了重复创建对象的开销，便于集中维护管理。  
4.采用Nginⅸ完成前端项目部署、采用Docker容器完成后端项目部署，并且使用宝塔面板对项目进行运维监控。  
5.使用JUnit Jupiter AP川的@Test注解和Assertions类实现对用户模块的单元测试，测试覆盖度达到90%。  
6.通过Spring Boot的多套application-{en-yml配置文件实现多环境，并通过指定spring.profiles.active:=prod实现生产环境部署。  
7.使用Nginⅸ网关统一接受前端页面和后端接口请求，并通过其proy_pasS反向代理配置解决跨域问题。  
