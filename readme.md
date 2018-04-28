# WNMP V1.0.0 说明文档
> 切勿将此环境用于生产环境，对于用于生产环境出现的任何问题作者概不负责。   
> 此套件的目的在于快速搭建一个windows上的nginx + php + mysql 的开发环境。  
> 对应的 nginx、mysql 和 php 版权归原作者所有，这里只是进行简单的组装。   
> RunHiddenConsole.exe 这个文件的作用是可以在后台运行nginx和mysql。   
> 有任何问题欢迎关注公众号“开发者那些事”(或者直接搜索“kfznxs”)，回复“wnmp” 或者直接留言。    
> power by zhangchongwang@163.com at 2018-04-28 

## 使用说明
- 下载 wamp-v1.0.0.zip
```
	git clone git@github.com:bill-wangwang/wnmp.git 
	#或者直接下载 https://codeload.github.com/bill-wangwang/wnmp/zip/master
```
- 解压 wamp-v1.0.0.zip 到任意目录（注意路径不能出现中文和空格，推荐路径为:  d:\wnmp ）
- 双击 “启动全部.bat” 即可启动全部服务
- 双击 “停止全部.bat” 即可停止全部服务
- 双击 “重启nginx.bat”即可重启nginx（一般用于修改或者新增虚拟站点配置时启用）
## 目录结构
```
├─logs  ------------------------- nginx日志目录 （必须有可写权限）
├─mysql-5.6.40-winx64  ---------- mysql目录
│  ├─data  ---------------------- mysql数据库数据存储目录（必须有可写权限）
├─nginx-1.14.0   ---------------- nginx目录
│  ├─conf  ---------------------- nginx配置目录
│  │  └─vhost ------------------- 虚拟站点配置目录（自动加载里面的*.conf）
├─php-7.1.17  ------------------- php目录
├─temp  ------------------------- nginx temp目录 （必须有可写权限）
└─web   ------------------------- 配置站点主目录
    └─test  --------------------- 测试虚拟主机目录
```

## 注意事项
- 此套件均为绿色软件，解压即可使用，免去繁琐的安装步骤
- 切勿将此环境用于生产环境
- mysql的root用户密码已经修改为123456
- 套件中php的版本为 php-7.1.17-nts， mysql的版本为 mysql-5.6.40-winx64，nginx的版本为 nginx-1.14.0