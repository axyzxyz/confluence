# confluence 安装，迁移
confluence - wiki 6.3.1 安装迁移教程


本项目提供confluence6.3.1的下载安装，及原服务迁移步骤（原服务程序java报错，服务无法重启，尝试重新搭建，并迁移）。

[confluence官方下载下载地址](https://www.atlassian.com/software/confluence/downloads/binary/atlassian-confluence-6.3.1-x64.bin)

```bash
wget https://www.atlassian.com/software/confluence/downloads/binary/atlassian-confluence-6.3.1-x64.bin
```

[confluence百度下载下载地址](https://pan.baidu.com/s/1skD5DQt) 密码：5vmk

### 破解文件列表
atlassian-extras-decoder-v2-3.2.jar  
atlassian-universal-plugin-manager-plugin-2.22.jar

### 安装教程
[参考博客](https://www.cnblogs.com/kevingrace/p/7607442.html)

### 迁移 or 还原
迁移还原时请选择第三个选项（从备份点还原），示意图如下：
![alt 还原点示意图](https://github.com/a001189/confluence/blob/master/907596-20170928192217606-575327038.jpg)

安装完成后，直接选择旧版本恢复，并导入备份文件zip压缩包，等待文件建立索引，数据库写入即可。
```bash
cd /var/atlassian/application-data/confluence/backups
sz backup*.zip
```
也可选择直接将文件，直接放入新服务提示的目录，即可。实测未成功，因此选择下载原备份文件，然后上传的方式，进行还原
