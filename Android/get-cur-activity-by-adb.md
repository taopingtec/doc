##    通过adb查看当前手机上显示的界面对应的activity



        linux:
        adb shell dumpsys activity | grep "mFocusedActivity"

        windows:
        adb shell dumpsys activity | findstr "mFocusedActivity"
        
