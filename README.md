# 《深入理解LFI漏洞》

本项目用来收集整理LFI漏洞的相关内容，包括LFI的利用方法工具或思路等。文件包含漏洞往往出现在PHP中，一般可以执行系统命令，包括LFI和RFI。文件读取漏洞和文件下载漏洞或者是路径穿越漏洞和文件包含漏洞很相似，往往不可以执行命令，只能读取有权限的文件。因为原理一样，所以都记录到了本仓库！作者：[ASTTeam](https://github.com/ASTTeam/LFI)

本项目创建于2020年12月1日，最近的一次更新时间为2022年3月7日。本项目会持续更新，直到海枯石烂！

- [01-LFI漏洞资源]()
- [02-LFI漏洞基础]()
- [03-LFI漏洞工具]()
- [04-LFI渗透测试]()
- [05-LFI代码审计]()
- [06-LFI漏洞赏金]()
- [07-LFI漏洞修复]()

## 01-LFI漏洞资源

- https://github.com/topics/LFI

一、LFI书籍资源

二、LFI培训演讲

三、LFI其他资源
- https://blog.csdn.net/weixin_34268753/article/details/89933140
- https://www.rcesecurity.com/2017/08/from-lfi-to-rce-via-php-sessions/
- https://outpost24.com/blog/from-local-file-inclusion-to-remote-code-execution-part-1
- https://sec-art.net/2021/10/27/exploiting-local-file-inclusion-lfi-vulnerability-with-proc-self-environ-method-lfi-attacks/
- https://xz.aliyun.com/t/6594

## 02-LFI漏洞基础

一、LFI漏洞概念

二、LFI漏洞原理

三、LFI漏洞分类

- PHP文件包含漏洞
- Java文件包含漏洞
- 任意文件读取漏洞
- 任意文件下载漏洞
- 本地文件包含
- 远程文件包含

四、LFI漏洞危害

五、LFI漏洞思考

- 文件包含漏洞，可以getshell吗？任意文件包含漏洞可以包含什么？
- PHP任意文件读取漏洞一定可以getshell吗？
- PHP文件包含漏洞如何getshell？
- Java的任意文件读取漏洞可以getshell吗？
- java文件包含-包含一个jsp文件可以执行命令吗？

## 03-LFI漏洞工具

- 如何开发一个文件包含漏洞的工具？

一、LFI Payload

- https://github.com/payloadbox/rfi-lfi-payload-list

二、LFI被动扫描

三、待整理
- https://github.com/LandGrey/ClassHound
- https://github.com/mzfr/liffy
- https://github.com/chrispetrou/FDsploit
- https://github.com/kostas-pa/LFITester
- https://github.com/BoxingOctopus/toxin
- https://github.com/emadshanab/LFI-Payload-List
- https://github.com/VainlyStrain/Vailyn
- https://github.com/aryanrtm/Crascan
- https://github.com/S1lkys/Auto_LFI
- https://github.com/sinsinology/phpinfo-Local-File-Inclusion
- https://github.com/hansmach1ne/lfimap
- https://github.com/abaykan/Labs
- https://github.com/machine1337/lfiscan
- https://github.com/redknight99/Lotsa_Fun_Included
- https://github.com/DSimsek000/finc
- https://github.com/jstigerwalt/WEB-Fuzz
- https://github.com/th3f0r3ign3r/Slifer
- https://github.com/stefan2200/Bud

## 04-LFI渗透测试

一、LFI漏洞挖掘

二、LFI危险参数

- &RealPath=、&readpath=、&FilePath=、&filepath=、&Path=、&path=、&Inputfile=、&inputfile=、&url=、&urls=、&Lang=、&dis=、&Data=、&data=、&readfile=、&ﬁlep=、&Src=、&src=、&menu=、META-INF= 、WEB-INF

三、LFI漏洞实战

四、LFI高级利用

## 05-LFI代码审计

一、LFI漏洞靶场

二、LFI审计原理

三、LFI危险函数

- 在PHP中：
  - 文件包括：include()、include_once()、require()、require_once()
  - 文件读取：readfile()、file_get_contents()、fopen()
- 在Java中：
- 在.NET中：

四、LFI漏洞分析

## 06-LFI漏洞赏金

- https://github.com/HoneTeam/LFI

## 07-LFI漏洞修复

## 08-LFI参考资源