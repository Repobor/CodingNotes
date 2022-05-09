# 在 Tomcat 中部署 war包 （服务器上）

1. 将项目打包，得到 war 文件
2. 在服务器上安装 [Tomcat](https://tomcat.apache.org/)
   1. 根据服务器以及项目实际版本下载 tar.gz / zip
   2. linux : `tar -zxvf apache-tomcat-$version.tar.gz`
3. 进入目录 apache-tomcat-$version
4. 将 war 包 放入 webapps 目录下
   1. 注意：建议将 war 包命名好，否则不便访问
5. 回到 bin 目录
   1. 执行 `./startup.sh` 启动服务器 默认端口是`8080`
   2. 执行 `./shutdown.sh` 关闭服务器
6. 访问项目 `http://example.org:8080/$warname/`

