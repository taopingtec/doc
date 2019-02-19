##    确认方法

###    1、检查如下地址是否存在

        C:/Users/(用户名)/.gradle/caches/modules-2/files-2.1
        
如果存在则有可能是存放地址

###    2、对于已配置好的Android Studio开发工程
检查工程的gradle配置，如下图：
![image2](/documents/Images/Android/gradle-cache/gradle-cache.png)

则缓存目录如下：
![image2](/documents/Images/Android/gradle-cache/gradle-cache2.png)

###    3、查看环境变量GRADLE_USER_HOME是否有配置
如果有配置，则一般为：

        %GRADLE_USER_HOME%/caches/modules-2/files-2.1    

###    4、gradle的安装目录
重点检查：

        %gradle安装目录%/caches/modules-2/files-2.1    


        

        