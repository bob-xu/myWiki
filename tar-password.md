#在Linux下打包tar文件时添加密码的方法

在当前目录下有一个pma目录的文件夹:

1、使用tar对文件压缩加密：


代码如下:
# tar -zcvf - pma|openssl des3 -salt -k password | dd of=pma.des3

完成将得到一个pma.des3的打包文件，用你设置的密码替换password 。
2、使用tar对加密文件解压：


复制代码
代码如下:
# dd if=pma.des3 |openssl des3 -d -k password|tar zxf -

注意：命令最后有”-”，它将释放所有的文件 。其中-k password可以不使用，这样执行完命令后会提示你输入密码，加上-k参数表示在程序中自动验证密码 。