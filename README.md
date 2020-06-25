# apache-tomcat-8
tomcat8.0版本源码阅读

修改启动配置：在`Bootstrap`类的启动类中添加启动参数
```
-Dfile.encoding=UTF8
-Dcatalina.home=catalina-home
-Dcatalina.base=catalina-home
-Djava.endorsed.dirs=catalina-home/endorsed
-Djava.io.tmpdir=catalina-home/temp
-Djava.util.logging.manager=org.apache.juli.ClassLoaderLogManager
-Djava.util.logging.config.file=catalina-home/conf/logging.properties
```
