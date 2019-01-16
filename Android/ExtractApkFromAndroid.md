##    导出步骤

###    1、找出应用的包名
执行如下命令获取手机中已安装的所有app的package信息：

        adb shell pm list package

获得如下结果

        package:com.android.emergency
        package:com.moji.zteweather
        package:com.mobimail.zte
        package:com.qualcomm.qti.RIDL
        package:com.smile.gifmaker        

###    2、找出apk的位置
执行如下命令，获取指定package对应apk文件的位置：

        adb shell pm path com.moji.zteweather
        
得到如下结果：

        package:/system/app/MojiWeather/MojiWeather.apk        
        

###    3、导出apk文件
执行如下命令，导出apk文件：

        adb pull /system/app/MojiWeather/MojiWeather.apk        

        