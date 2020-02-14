

# Swagger-Sero （swagger-ui）

> 为了方便部署[editor.swagger.io]( http://editor.swagger.io/ )的设计成果，在[swagger-ui]( https://github.com/swagger-api/swagger-ui )上做了一些修改，实现多设计文档的部署。

 ![img](./swagger.jpg) 



## 部署

- 首先，你得有一个nginx、tomcat之类的Web部署容器；

- Clone代码到本地，并将它部署到Web容器中；

  ~~~
  git clone https://github.com/lebean/swagger-sero.git
  ~~~

- 将[editor.swagger.io]( http://editor.swagger.io/ )中的设计成果导出为json；

- 复制成果json到swagger-sero目录下的json文件夹中，在json文件夹中可以包含多个成果json文件；

*做到这些，就完成了APIS-DOC以及API设计成果的部署了*



## 访问

【URL】http://{host}/swagger-sero/index.html?doc={json文件名}

~~~
http://my-service/swagger-sero/index.html?doc=my-api.json
~~~

