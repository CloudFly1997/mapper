# mapper
通用Mapper代码生成器

## 使用步骤
- 下载项目
- 使用idea打开工程
- 修改/main/resources/config.properties文件
  ```properties
  #数据库连接字段
  url=jdbc:mysql://192.168.1.100:3306/mapper?useUnicode=true&characterEncoding=utf8
  driverClassName=com.mysql.jdbc.Driver
  username=root
  password=root
  tableName=tabple_emp
  beanName=Employee

  #通用Mapper逆向工程生成文件包名
  modelPackage=com.wyf.bean
  mapperPackage=com.wyf.mappers
  mapperXmlPackage=com.wyf.mappers
  ```
- 在 pom.xml 这一级目录的命令行窗口执行`mvn mybatis-generator:generate`即可