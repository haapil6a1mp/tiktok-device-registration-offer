🌟✨ **Elevate Your Business with Our Cutting-Edge Solutions** ✨🌟

Presenting a 🔐 **Trustworthy** and 🚀 **Innovative** proposal for your business needs! Leverage the power of our top-notch features:

🎯 **TikTok X-Gorgon, X-Argus, and TTEncrypt algorithms (unidbg)** Experience unparalleled security and performance with these advanced algorithms, perfect for your business! 💪

🤖 **Device Registration** Fully automate new devices registration process with our advanced device registration solution! 📱

⚙️ **Autoreg** Automate your accounts registration process with ease, saving time and resources! ⏰

🐍 **Python API Library (adaptable to various application versions)** Stay ahead of the curve with our flexible and adaptable API library for all your application needs! 🌐

💼 What We Offer:

- 🌐 API/Source Code

- 🎥 Demonstration Accessible

- 📧 Inquiries via email: polk9pjuar@gmail.com

- 🕐 **Prompt Response Guaranteed Within 24 Hours!**

Don't miss this opportunity to enhance your business with our cutting-edge solutions! 🌟 Contact us now! 📩

---

---

---







# 部署文档

> 基于抖音版本12.5.0 so文件

#### 依赖环境

Java 1.8 Maven

##### 安装 Maven

```
wget http://mirrors.tuna.tsinghua.edu.cn/apache/maven/maven-3/3.3.9/binaries/apache-maven-3.3.9-bin.tar.gz
```

````
tar -zxvf apache-maven-3.3.9-bin.tar.gz
````

````
mv apache-maven-3.3.9 /usr/local/maven
````

````
vim /etc/profile
````

在/etc/profile文件末尾增加以下配置：

````
M2_HOME=/usr/local/maven
export PATH=${M2_HOME}/bin:${PATH}
````

重载/etc/profile这个文件

````
source /etc/profile
````

检查安装

```
mvn -v
```



### 一键代码Jar包

```
cd 目录
```
```
mvn clean install -DskipTests
```
```
cd target
```
```
java -jar douyin-spider-0.0.1-SNAPSHOT.jar
```
---
访问地址: http://localhost:8022/register

---

### 注意

服务器需要开9022端口。  

跑脚本需要间隔3秒，否则可能出现抖音风控  

##### 其他
清理nohup.out 日志
```
cat /dev/null > /www/wwwroot/douyin-register-spider/target/nohup.out
```

此代码仅供学习参考,设备信息版本太老,利用率很低的.
如果访问接口出现3072表示还需要滑块验证

#### 常见问题

如果注册出来的大批量设备无法使用(获取不到数据),可以尝试使用真机设备标识. 如果还是不行说明接口风控升级了,需要新版的算法
