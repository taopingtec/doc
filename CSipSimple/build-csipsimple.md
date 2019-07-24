###    1、选择module “app”，点击运行，报NDK的问题
错误提示：

        14:20:12.474 [ERROR] [org.gradle.BuildExceptionReporter] 
        14:20:12.474 [ERROR] [org.gradle.BuildExceptionReporter] FAILURE: Build failed with an exception.
        14:20:12.474 [ERROR] [org.gradle.BuildExceptionReporter] 
        14:20:12.474 [ERROR] [org.gradle.BuildExceptionReporter] * What went wrong:
        14:20:12.474 [ERROR] [org.gradle.BuildExceptionReporter] Execution failed for task ':app:compileDebugNdk'.
        14:20:12.474 [ERROR] [org.gradle.BuildExceptionReporter] > Error: NDK integration is deprecated in the current plugin.  Consider trying the new experimental plugin.  For details, see http://tools.android.com/tech-docs/new-build-system/gradle-experimental.  Set "android.useDeprecatedNdk=true" in gradle.properties to continue using the current NDK integration.
        14:20:12.474 [ERROR] [org.gradle.BuildExceptionReporter] 
        14:20:12.474 [ERROR] [org.gradle.BuildExceptionReporter] * Try:
        14:20:12.474 [ERROR] [org.gradle.BuildExceptionReporter] Run with --stacktrace option to get the stack trace. 
        
解决思路：不编译pjsip
解决方法：
    1、下载CSipSimple-0.04-01.apk，解压后，将lib考入工程对应的目录
    2、下载pjsip的jni代码https://sourceforge.net/projects/pjsip-jni/，并放入工程