**环境安装**

1. 安装python 环境（mac和linux系统自带不需要安装)
2. 命令行执行：python -m SimpleHTTPServer \<port\> 端口默认8000
* 例如：python -m SimpleHTTPServer 8010

>**模拟接口**

> - 1. 创建接口文件夹
> - 2. cd path/of/接口目录
> - 3. python -m SimpleHTTPServer \<port\>
> - 4. 访问接口：http://localhost:\<port\>/JieKouWenJian.html <font color='red'>&#160;&#160;Note:文件一定使用html结尾，否则会提示下载</font>
> - * 例如：http://localhost:8000/login.html?username='hello'&passwd='world'