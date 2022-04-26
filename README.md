## 安装

### 安装方式 (GO MOD方式安装,已移除 GOPATH方式安装说明，需要的请查看 tag v1.0.1)

#### 1、安装beego v2.0.1和bee v2.0.2
参考[Beego](https://beego.me/docs/install/)和[Bee](https://beego.me/docs/install/bee.md)安装手册

#### 2、clone 项目到本地 GOPATH src目录之外的路径下
```
GitHub:   https://github.com/huanguang/go-base.git
```
或
```
码云:   https://gitee.com/lhg002/go-base.git
```


#### 3、配置数据库
```
将目录中go-admin.sql文件导入mysql数据库

更改根目录下的config.yaml文件内的数据库连接信息
```

#### 4、安装项目依赖
```
目录下 go mod tidy 将自动下载依赖包
```

### 通过上面方式安装后,接下来

#### 运行系统
```
直接运行go run main.go，或者使用bee run在项目下运行，开始进行调试开发
```

#### 访问后台
访问`/admin/index/index`，默认超级管理员的账号:`admin`,密码：`123456`。


## 注意！！！
当前最新master版本beego v2.0.1框架的版本，如果需要beego1.x 版本的请下载 tag v1.0.1 版本，因 Beego 2.x 的XSRF只支持 HTTPS 协议，所有app.conf配置中默认关闭了XSRF安全过滤，如有需要请手动开启,因beego v2.X版本和 beego v1.x版本区别较大，请根据beego最新手册进行开发使用。

技术交流QQ：923414405

