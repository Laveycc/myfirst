第一步：修改tomcat-users.xml配置文件，配置用户、密码和权限
```
<role rolename="manager-gui" />
<role rolename="manager-script" />
<user username="tomcat" password="tomcat" roles="manager-gui, manager-script"/>
```
第二步：在pom文件中配置tomcat插件。
![这里写图片描述](http://img.blog.csdn.net/20170604135923777?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQva29uZ19sZXY=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
第三步：部署
初次部署可以使用 "tomcat7:deploy" 命令
如果已经部署过使用 "tomcat7:redeploy" 命令

![这里写图片描述](http://img.blog.csdn.net/20170604140101044?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQva29uZ19sZXY=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
<font color="red">注意：</font>
先启动tomcat，再进行部署。
部署完成后，就可以通过部署的网址进行访问了。
