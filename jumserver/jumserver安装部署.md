**环境要求：**

| 资源  | 最低要求 |
| :-: | ---- |
| CPU | 2C   |
| 内存  | 4G   |
| 硬盘  | 40G  |
操作系统：
CentOS      Ubuntu


二进制安装
```
#切换目录
cd /opt

curl -sSL https://resource.fit2cloud.com/jumpserver/jumpserver/releases/latest/download/quick_start.sh | bash
```

opt目录下会自己创建四个目录

cni/    containerd/    jumpserver/    jumpserver-installer-v4.10.16/

![[Pasted image 20260601150905.png]]

jumserver基础命令：
```
安装：

./jmsctl.sh   install

切换到jumpserver-installer-v4.10.16/目录下启动：

cd  jumpserver-installer-v4.10.16/

./jmsctl.sh   start

停止：

./jmsctl.sh   down
```

部署完就可以进入浏览器输入宿主机IP地址（默认是80端口）即可登录
登录页面输入账号密码：（默认的账户密码是 admin / ChangeMe）
![[Pasted image 20260601151718.png]]
进来之后修改密码：
![[Pasted image 20260601152207.png]]
点开个人信息找到更新密码：
![[Pasted image 20260601152245.png]]
输入原密码并修改新密码：
![[Pasted image 20260601152317.png]]
返回首页，找到资产列表：
![[Pasted image 20260601152414.png]]
点击创建：
![[Pasted image 20260601152436.png]]
选择对应主机（Linux）：
![[Pasted image 20260601152523.png]]
红框当中写入：
名称：写虚拟机安装的操作系统（推荐）
IP：宿主机IP地址
节点：默认
![[Pasted image 20260601152608.png]]
点击新建：
名称：写虚拟机安装的操作系统（推荐）
用户名：宿主机的名称
密码：宿主机密码
然后点击确认即可
![[Pasted image 20260601152813.png]]
最后点击提交即可并找到资产授权
![[Pasted image 20260601153038.png]]
点击创建：
![[Pasted image 20260601153102.png]]
名称：自定义
用户：默认
![[Pasted image 20260601153142.png]]
资产：选择刚刚所创建的
节点：默认
![[Pasted image 20260601153232.png]]
最后提交即可
![[Pasted image 20260601153313.png]]
返回首页点击终端即可连接：
![[Pasted image 20260601153343.png]]








































