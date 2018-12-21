# smtp2webhook

## 使用说明

1. 安装node.js，开发时用的版本是10.14.2，其他版本应该问题不大。

略

2. 安装依赖

$ npm i

3. 修改配置文件config.js

略

4. 修改域名记录

在直接指向域名的mx记录之前，需要先添加域名的a记录。这里以aaa.com为例。

将mx1.aaa.com, mx2.aaa.com, mx3.aaa.com等分别指向负载均衡里的每一台机器。

然后创建aaa.com的多条mx记录，分别指向mx1.aaa.com, mx2.aaa.com, ...

5. 从任意邮箱向anybody@aaa.com发送测试邮件