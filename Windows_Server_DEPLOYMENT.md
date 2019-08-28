# Windows-Server 部署方案 （IIS + Django）

## IIS 开启和配置
1. 控制面板 > 程序和功能 > 启动或关闭Windows功能

![image](https://github.com/awesome33rabbit/DEPLOYMENT/blob/master/static/Windows-Server/1.png)

![image](https://github.com/awesome33rabbit/DEPLOYMENT/blob/master/static/Windows-Server/2.png)
2. 开启IIS

![image](https://github.com/awesome33rabbit/DEPLOYMENT/blob/master/static/Windows-Server/3.png)
3. 验证IIS是否成功开启
    - 开启IIS后，会有默认的网站运行。
    
![image](https://github.com/awesome33rabbit/DEPLOYMENT/blob/master/static/Windows-Server/4.png)
    - 浏览器输入 http://localhost:80/，出现默认页面。
    
![image](https://github.com/awesome33rabbit/DEPLOYMENT/blob/master/static/Windows-Server/5.png)

## Django 项目添加到IIS
1. 安装 wfastcgi
    ```pip install wfastcgi```
    - 安装完成后，管理员权限运行命令提示符，输入wfastcgi-enable显示成功，则完成下载；出现异常，可输入wfast-disable，之后重新运行wfastcgi-enable
2. IIS上创建网站

![image](https://github.com/awesome33rabbit/DEPLOYMENT/blob/master/static/Windows-Server/6.png)
3. 创建程序映射，即fcgi程序

![image](https://github.com/awesome33rabbit/DEPLOYMENT/blob/master/static/Windows-Server/7.png)
4. 添加环境变量

![image](https://github.com/awesome33rabbit/DEPLOYMENT/blob/master/static/Windows-Server/8.png)

![image](https://github.com/awesome33rabbit/DEPLOYMENT/blob/master/static/Windows-Server/9.png)

![image](https://github.com/awesome33rabbit/DEPLOYMENT/blob/master/static/Windows-Server/10.png)
