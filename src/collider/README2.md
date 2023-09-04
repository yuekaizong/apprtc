1.在collider目录下执行：
go mod init collider
2.编辑go.mod文件
添加依赖:
require golang.org/x/net v0.14.0
3.更改程序入口：
mv ./collidermian/main.go .
4.更改项目结构：
将import里面的"collider"全部替换为"collider/collidertest"
5.更新项依赖： 
go get
6.编译出可执行文件
go build
7.启动collider服务
/collidermain -port=8089 -tls=true