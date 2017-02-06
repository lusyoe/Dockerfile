FROM tomcat:latest

MAINTAINER luhaoyuan <lusyoe@163.com>

# 远程登录tomcat控制台与远程部署用户配置
ADD tomcat-users.xml /usr/local/tomcat/conf/

# 默认server设置，修改默认首页项目
ADD server.xml /usr/local/tomcat/conf/


CMD ["catalina.sh", "run"]
