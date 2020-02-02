####    1、更换pull源
vi  /etc/docker/daemon.json 
我用的是ubuntu16.04系统，安装完docker之后，并没有daemon.json这个文件，可以通过vi编辑保存的方式创建这个文件，在文件中添加如下内容：

        {
            "registry-mirrors":[
                "https://kfwkfulq.mirror.aliyuncs.com",
                "https://2lqq34jg.mirror.aliyuncs.com",
                "https://pee6w651.mirror.aliyuncs.com",
                "http://hub-mirror.c.163.com",
                "https://docker.mirrors.ustc.edu.cn",
                "https://registry.docker-cn.com"
            ]
        }

####    2、加载配置文件

        systemctl daemon-reload
    
####    3、重启docker服务

        systemctl restart docker


####   参考资料
* [https://bbs.huaweicloud.com/blogs/141435](https://bbs.huaweicloud.com/blogs/141435)

